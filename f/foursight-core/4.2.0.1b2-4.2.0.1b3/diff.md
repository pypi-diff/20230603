# Comparing `tmp/foursight_core-4.2.0.1b2.tar.gz` & `tmp/foursight_core-4.2.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.2.0.1b2.tar", max compression
+gzip compressed data, was "foursight_core-4.2.0.1b3.tar", max compression
```

## Comparing `foursight_core-4.2.0.1b2.tar` & `foursight_core-4.2.0.1b3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1083 2023-06-01 22:56:44.423182 foursight_core-4.2.0.1b2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-01 22:56:44.428854 foursight_core-4.2.0.1b2/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-01 22:56:44.428926 foursight_core-4.2.0.1b2/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-01 22:56:44.428975 foursight_core-4.2.0.1b2/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-06-01 22:56:44.429358 foursight_core-4.2.0.1b2/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-01 22:56:44.429443 foursight_core-4.2.0.1b2/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-01 22:56:44.429510 foursight_core-4.2.0.1b2/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-01 22:56:44.429564 foursight_core-4.2.0.1b2/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-01 22:56:44.429683 foursight_core-4.2.0.1b2/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-01 22:56:44.429780 foursight_core-4.2.0.1b2/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4476 2023-06-01 22:56:44.429859 foursight_core-4.2.0.1b2/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-01 22:56:44.429921 foursight_core-4.2.0.1b2/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-01 22:56:44.429986 foursight_core-4.2.0.1b2/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-01 22:56:44.430060 foursight_core-4.2.0.1b2/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-01 22:56:44.430116 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-01 22:56:44.430181 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-01 22:56:44.430250 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-01 22:56:44.430319 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-01 22:56:44.430396 foursight_core-4.2.0.1b2/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-01 22:56:44.430459 foursight_core-4.2.0.1b2/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-01 22:56:44.430544 foursight_core-4.2.0.1b2/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-01 22:56:44.430637 foursight_core-4.2.0.1b2/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-01 22:56:44.430719 foursight_core-4.2.0.1b2/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-01 22:56:44.430804 foursight_core-4.2.0.1b2/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-01 22:56:44.430943 foursight_core-4.2.0.1b2/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-06-01 22:56:44.431016 foursight_core-4.2.0.1b2/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-01 22:56:44.431090 foursight_core-4.2.0.1b2/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-01 22:56:44.431156 foursight_core-4.2.0.1b2/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-01 22:56:44.431211 foursight_core-4.2.0.1b2/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-01 22:56:44.431385 foursight_core-4.2.0.1b2/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-01 22:56:44.431609 foursight_core-4.2.0.1b2/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-01 22:56:44.431723 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-01 22:56:44.431939 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-01 22:56:44.432016 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-01 22:56:44.432132 foursight_core-4.2.0.1b2/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-01 22:56:44.432264 foursight_core-4.2.0.1b2/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-01 22:56:44.432340 foursight_core-4.2.0.1b2/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-01 22:56:44.432411 foursight_core-4.2.0.1b2/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-01 22:56:44.432474 foursight_core-4.2.0.1b2/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-01 22:56:44.432538 foursight_core-4.2.0.1b2/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-01 22:56:44.432603 foursight_core-4.2.0.1b2/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-01 22:56:44.432670 foursight_core-4.2.0.1b2/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-01 22:56:44.432733 foursight_core-4.2.0.1b2/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-01 22:56:44.432818 foursight_core-4.2.0.1b2/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-01 22:56:44.432903 foursight_core-4.2.0.1b2/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    79982 2023-06-01 22:56:51.122411 foursight_core-4.2.0.1b2/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-01 22:56:44.433257 foursight_core-4.2.0.1b2/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-01 22:56:44.433344 foursight_core-4.2.0.1b2/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-01 22:56:51.122756 foursight_core-4.2.0.1b2/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-01 22:56:44.433545 foursight_core-4.2.0.1b2/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-01 22:56:44.433609 foursight_core-4.2.0.1b2/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-01 22:56:44.433696 foursight_core-4.2.0.1b2/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-01 22:56:44.433762 foursight_core-4.2.0.1b2/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-01 22:56:44.433809 foursight_core-4.2.0.1b2/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-01 22:56:44.434363 foursight_core-4.2.0.1b2/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1933280 2023-06-01 22:56:51.139496 foursight_core-4.2.0.1b2/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-01 22:56:44.444816 foursight_core-4.2.0.1b2/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-01 22:56:44.444904 foursight_core-4.2.0.1b2/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-01 22:56:44.444966 foursight_core-4.2.0.1b2/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-01 22:56:44.445073 foursight_core-4.2.0.1b2/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-01 22:56:44.445156 foursight_core-4.2.0.1b2/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-01 22:56:44.445259 foursight_core-4.2.0.1b2/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-01 22:56:44.445320 foursight_core-4.2.0.1b2/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-01 22:56:44.445402 foursight_core-4.2.0.1b2/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-01 22:56:44.445471 foursight_core-4.2.0.1b2/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-01 22:56:44.445653 foursight_core-4.2.0.1b2/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-01 22:56:44.445766 foursight_core-4.2.0.1b2/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-01 22:56:44.445844 foursight_core-4.2.0.1b2/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-01 22:56:44.445927 foursight_core-4.2.0.1b2/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-01 22:56:44.445997 foursight_core-4.2.0.1b2/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-01 22:56:44.446057 foursight_core-4.2.0.1b2/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-01 22:56:44.446124 foursight_core-4.2.0.1b2/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-01 22:56:44.446212 foursight_core-4.2.0.1b2/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-01 22:56:44.446266 foursight_core-4.2.0.1b2/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1626 2023-06-01 22:56:51.140511 foursight_core-4.2.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b2/setup.py
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-03 18:19:58.330926 foursight_core-4.2.0.1b3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-03 18:19:58.335866 foursight_core-4.2.0.1b3/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-03 18:19:58.335933 foursight_core-4.2.0.1b3/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-03 18:19:58.335986 foursight_core-4.2.0.1b3/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-06-03 18:19:58.336395 foursight_core-4.2.0.1b3/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-03 18:19:58.336479 foursight_core-4.2.0.1b3/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-03 18:19:58.336542 foursight_core-4.2.0.1b3/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-03 18:19:58.336601 foursight_core-4.2.0.1b3/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-03 18:19:58.336727 foursight_core-4.2.0.1b3/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-03 18:19:58.336820 foursight_core-4.2.0.1b3/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4476 2023-06-03 18:19:58.336895 foursight_core-4.2.0.1b3/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-03 18:19:58.336958 foursight_core-4.2.0.1b3/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-03 18:19:58.337029 foursight_core-4.2.0.1b3/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-03 18:19:58.337109 foursight_core-4.2.0.1b3/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:19:58.337171 foursight_core-4.2.0.1b3/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-03 18:19:58.337249 foursight_core-4.2.0.1b3/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-03 18:19:58.337319 foursight_core-4.2.0.1b3/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-03 18:19:58.337402 foursight_core-4.2.0.1b3/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-03 18:19:58.337477 foursight_core-4.2.0.1b3/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-03 18:19:58.337539 foursight_core-4.2.0.1b3/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-03 18:19:58.337629 foursight_core-4.2.0.1b3/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-03 18:19:58.337726 foursight_core-4.2.0.1b3/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-03 18:19:58.337807 foursight_core-4.2.0.1b3/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-03 18:19:58.337888 foursight_core-4.2.0.1b3/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-03 18:19:58.338023 foursight_core-4.2.0.1b3/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5215 2023-06-03 18:20:07.463986 foursight_core-4.2.0.1b3/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-03 18:19:58.338167 foursight_core-4.2.0.1b3/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-03 18:19:58.338229 foursight_core-4.2.0.1b3/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-03 18:19:58.338279 foursight_core-4.2.0.1b3/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-03 18:19:58.338456 foursight_core-4.2.0.1b3/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-03 18:19:58.338556 foursight_core-4.2.0.1b3/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-03 18:19:58.338675 foursight_core-4.2.0.1b3/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-03 18:19:58.338887 foursight_core-4.2.0.1b3/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-03 18:19:58.338971 foursight_core-4.2.0.1b3/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-03 18:19:58.339105 foursight_core-4.2.0.1b3/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-03 18:19:58.339248 foursight_core-4.2.0.1b3/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-03 18:19:58.339332 foursight_core-4.2.0.1b3/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-03 18:19:58.339408 foursight_core-4.2.0.1b3/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-03 18:19:58.339490 foursight_core-4.2.0.1b3/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-03 18:19:58.339566 foursight_core-4.2.0.1b3/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-03 18:19:58.339636 foursight_core-4.2.0.1b3/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-03 18:19:58.339706 foursight_core-4.2.0.1b3/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-03 18:19:58.339778 foursight_core-4.2.0.1b3/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-03 18:19:58.339871 foursight_core-4.2.0.1b3/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-03 18:19:58.339955 foursight_core-4.2.0.1b3/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    80447 2023-06-03 18:20:07.464587 foursight_core-4.2.0.1b3/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-03 18:19:58.340310 foursight_core-4.2.0.1b3/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-03 18:19:58.340399 foursight_core-4.2.0.1b3/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-03 18:20:07.464929 foursight_core-4.2.0.1b3/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-03 18:19:58.340592 foursight_core-4.2.0.1b3/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-03 18:19:58.340664 foursight_core-4.2.0.1b3/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-03 18:19:58.340750 foursight_core-4.2.0.1b3/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-03 18:19:58.340813 foursight_core-4.2.0.1b3/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-03 18:19:58.340861 foursight_core-4.2.0.1b3/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-03 18:19:58.341446 foursight_core-4.2.0.1b3/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1934060 2023-06-03 18:20:07.481579 foursight_core-4.2.0.1b3/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-03 18:19:58.349696 foursight_core-4.2.0.1b3/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-03 18:19:58.349776 foursight_core-4.2.0.1b3/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-03 18:19:58.349837 foursight_core-4.2.0.1b3/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-03 18:19:58.349930 foursight_core-4.2.0.1b3/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-03 18:19:58.350000 foursight_core-4.2.0.1b3/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-03 18:19:58.350093 foursight_core-4.2.0.1b3/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-03 18:19:58.350143 foursight_core-4.2.0.1b3/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-03 18:19:58.350219 foursight_core-4.2.0.1b3/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-03 18:19:58.350290 foursight_core-4.2.0.1b3/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-03 18:19:58.350463 foursight_core-4.2.0.1b3/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-03 18:19:58.350568 foursight_core-4.2.0.1b3/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-03 18:19:58.350640 foursight_core-4.2.0.1b3/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-03 18:19:58.350722 foursight_core-4.2.0.1b3/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-03 18:19:58.350788 foursight_core-4.2.0.1b3/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-03 18:19:58.350843 foursight_core-4.2.0.1b3/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-03 18:19:58.350907 foursight_core-4.2.0.1b3/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-03 18:19:58.350993 foursight_core-4.2.0.1b3/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-03 18:19:58.351044 foursight_core-4.2.0.1b3/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1626 2023-06-03 18:20:07.482355 foursight_core-4.2.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b3/setup.py
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b3/PKG-INFO
```

### Comparing `foursight_core-4.2.0.1b2/LICENSE.txt` & `foursight_core-4.2.0.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/abstract_connection.py` & `foursight_core-4.2.0.1b3/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/app_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/buckets.py` & `foursight_core-4.2.0.1b3/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/check_schema.py` & `foursight_core-4.2.0.1b3/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/check_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/ecs_checks.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/scaling_checks.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/checks/test_checks.py` & `foursight_core-4.2.0.1b3/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/decorators.py` & `foursight_core-4.2.0.1b3/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/deploy.py` & `foursight_core-4.2.0.1b3/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/environment.py` & `foursight_core-4.2.0.1b3/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/es_connection.py` & `foursight_core-4.2.0.1b3/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/exceptions.py` & `foursight_core-4.2.0.1b3/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/fs_connection.py` & `foursight_core-4.2.0.1b3/foursight_core/fs_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,28 @@
             'es': es
         }
         # FOURFRONT information
         self.ff_server = fs_environ_info['fourfront']
         self.ff_env = fs_environ_info['ff_env']
         self.ff_es = fs_environ_info['es']
         self.ff_bucket = fs_environ_info['bucket']
+        self.redis = None
+        self.redis_url = None
         try:
             if 'redis' in fs_environ_info:
-                self.redis = RedisBase(create_redis_client(url=fs_environ_info['redis']))
+                self.redis_url = fs_environ_info['redis']
+                self.redis = RedisBase(create_redis_client(url=self.redis_url))
             elif 'REDIS_HOST' in os.environ:  # temporary patch in until env config is fully sorted - Will
-                self.redis = RedisBase(create_redis_client(url=os.environ['REDIS_HOST']))
-            else:
-                self.redis = None
+                self.redis_url = os.environ['REDIS_HOST']
+                self.redis = RedisBase(create_redis_client(url=self.redis_url))
         except redis.exceptions.ConnectionError:
             PRINT('Cannot connect to Redis')
             PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
         PRINT(self.redis)
-        PRINT(os.environ.get('REDIS_HOST', 'no-redis-host'))
+        PRINT(self.redis_url)
         if not test:
             self.ff_s3 = s3Utils(env=self.ff_env)
             try:  # TODO: make this configurable from env variables?
                 self.ff_keys = self.ff_s3.get_access_keys('access_key_foursight')
             except Exception as e:
                 raise Exception('Could not initiate connection to Fourfront; it is probably a bad ff_env. '
                       'You gave: %s. Error message: %s' % (self.ff_env, str(e)))
```

### Comparing `foursight_core-4.2.0.1b2/foursight_core/identity.py` & `foursight_core-4.2.0.1b3/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/mapping.json` & `foursight_core-4.2.0.1b3/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/package.py` & `foursight_core-4.2.0.1b3/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/auth.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/auth0_config.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_network.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_s3.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/checks.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/cognito.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/encryption.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/envs.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/gac.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/misc_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/react_api.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,17 @@
         """
         domain, context = app.core.get_domain_and_context(request)
         stage_name = app.core.stage.get_stage()
         default_env = self._envs.get_default_env()
         aws_credentials = self._auth.get_aws_credentials(env or default_env)
         portal_url = app.core.get_portal_url(env or default_env)
         portal_base_url = get_base_url(portal_url)
+        connection = app.core.init_connection(env)
+        redis_url = connection.redis_url
+        redis = connection.redis
         response = {
             "app": {
                 "title": app.core.html_main_title,
                 "package": app.core.APP_PACKAGE_NAME,
                 "stage": stage_name,
                 "version": app.core.get_app_version(),
                 "domain": domain,
@@ -352,18 +355,27 @@
                 "launched": app.core.init_load_time,
                 "deployed": app.core.get_lambda_last_modified(),
                 "accounts_file": self._get_accounts_file(),
                 "accounts_file_from_s3": self._get_accounts_file_from_s3()
             },
             "versions": self._get_versions_object(),
             "portal": {
-                "url": app.core.get_portal_url(env or default_env),
+                "url": portal_url,
                 "health_url": portal_base_url + "/health?format=json",
                 "health_ui_url": portal_base_url + "/health"
             },
+            "resources": {
+                "es": app.core.host,
+                "foursight": self.foursight_instance_url(request),
+                "portal": portal_url,
+                "rds": os.environ["RDS_HOSTNAME"],
+                "redis": redis_url,
+                "redis_running": redis is not None,
+                "sqs": self._get_sqs_queue_url(),
+            },
             "s3": {
                 "bucket_org": os.environ.get("ENCODED_S3_BUCKET_ORG", os.environ.get("S3_BUCKET_ORG", None)),
                 "global_env_bucket": os.environ.get("GLOBAL_ENV_BUCKET", os.environ.get("GLOBAL_BUCKET_ENV", None)),
                 "encrypt_key_id": os.environ.get("S3_ENCRYPT_KEY_ID", None)
             }
         }
         return response
```

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/react_api_base.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/react_routes.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/react_ui.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/ui/index.html` & `foursight_core-4.2.0.1b3/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.2.0.1b3/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.2.0.1b3/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.62ec1490.js.LICENSE.txt */
+/*! For license information please see main.b7685537.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -59315,71 +59315,82 @@
                     f = void 0 === d ? null : d,
                     p = e.elasticsearch,
                     h = void 0 !== p && p,
                     g = e.python,
                     y = void 0 !== g && g,
                     m = (e.chalice, e.check),
                     v = void 0 !== m && m,
-                    M = e.link,
-                    b = void 0 === M ? null : M,
-                    j = e.optional,
-                    w = void 0 !== j && j,
-                    x = e.portalCertificate,
+                    M = e.nocheck,
+                    b = void 0 !== M && M,
+                    j = e.link,
+                    w = void 0 === j ? null : j,
+                    x = e.optional,
                     N = void 0 !== x && x,
-                    I = e.portalAccessKey,
+                    I = e.portalCertificate,
                     D = void 0 !== I && I,
-                    S = e.apiCache,
-                    L = void 0 !== S && S;
-                var k = {
+                    S = e.portalAccessKey,
+                    L = void 0 !== S && S,
+                    k = e.apiCache,
+                    C = void 0 !== k && k;
+                var E = {
                         fontSize: "11pt",
                         fontFamily: o ? "monospace" : "inherit",
                         fontWeight: "bold",
                         wordWrap: "break-word",
                         cursor: a ? "copy" : "inherit",
                         align: "left"
                     },
-                    C = a ? {
+                    _ = a ? {
                         onClick: function() {
                             return Yr.Copy(t)
                         }
                     } : {},
-                    E = v ? (0, Kr.jsxs)("span", {
+                    T = v ? (0, Kr.jsxs)("span", {
                         children: ["\xa0", (0, Kr.jsx)("b", {
                             style: {
                                 fontSize: "13pt",
                                 color: "green"
                             },
                             children: Fr.Check
                         })]
                     }) : (0, Kr.jsx)("span", {}),
-                    _ = c ? (0, Kr.jsxs)("span", {
+                    A = b ? (0, Kr.jsxs)("span", {
+                        children: ["\xa0", (0, Kr.jsx)("b", {
+                            style: {
+                                fontSize: "13pt",
+                                color: "red"
+                            },
+                            children: Fr.X
+                        })]
+                    }) : (0, Kr.jsx)("span", {}),
+                    O = c ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://pypi.org/project/" + t + "/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "pypi",
                                 src: Ut.PyPi(),
                                 height: "21"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    T = f ? (0, Kr.jsxs)("span", {
+                    z = f ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://github.com/" + f + "/" + ("dcicutils" === t ? "utils" : t) + "/releases/tag/" + ("chalice" !== t ? "v" : "") + n,
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.GitHub(),
                                 height: "15"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    A = h ? (0, Kr.jsxs)("span", {
+                    U = h ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://www.elastic.co/guide/en/elasticsearch/reference/".concat(function(e) {
                                 var t = null === e || void 0 === e ? void 0 : e.split(".");
                                 return (null === t || void 0 === t ? void 0 : t.length) >= 2 ? t[0] + "." + t[1] : e
                             }(n), "/release-notes-").concat(n, ".html"),
@@ -59389,33 +59400,33 @@
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.ElasticsearchLogo(),
                                 height: "18"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    O = y ? (0, Kr.jsxs)("span", {
+                    P = y ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://docs.python.org/release/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "python",
                                 src: Ut.Python(),
                                 height: "19"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    z = (0, Kr.jsx)("span", {});
+                    R = (0, Kr.jsx)("span", {});
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         style: {
                             marginTop: "1px"
                         },
-                        children: !w || n ? (0, Kr.jsxs)("div", {
+                        children: !N || n ? (0, Kr.jsxs)("div", {
                             className: "row",
                             children: [(0, Kr.jsx)("div", {
                                 className: "col-sm-" + u,
                                 children: (0, Kr.jsxs)("div", {
                                     style: {
                                         fontSize: "11pt",
                                         fontFamily: "inherit",
@@ -59424,403 +59435,322 @@
                                         align: "left"
                                     },
                                     children: [t, ":"]
                                 })
                             }), (0, Kr.jsxs)("div", Ye(Ye({
                                 id: t,
                                 className: "col-sm-8",
-                                style: k,
+                                style: E,
                                 align: "left"
-                            }, C), {}, {
-                                children: [_, T, A, O, z, b && n ? (0, Kr.jsx)("span", {
+                            }, _), {}, {
+                                children: [O, z, U, P, R, w && n ? (0, Kr.jsx)("span", {
                                     children: (0, Kr.jsx)(Oe, {
-                                        to: b,
+                                        to: w,
                                         children: n
                                     })
                                 }) : (0, Kr.jsxs)("span", {
                                     children: [st.IsNonEmptyObject(n) ? (0, Kr.jsx)(Kr.Fragment, {
                                         children: n
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
                                         children: n || (0, Kr.jsx)("span", {
                                             children: Fr.EmptySet
                                         })
-                                    }), D && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), L && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/portal_access_key"),
                                             children: "View Details"
                                         })]
-                                    }), N && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), D && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/certificates"),
                                             children: "View Certificate"
                                         })]
-                                    }), L && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), C && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/apicache"),
                                             children: "View API Cache"
                                         })]
                                     })]
-                                }), E]
+                                }), T, A]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
             Ds = function() {
-                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = ta(),
-                    B = Xi("/info"),
-                    F = a((0, t.useState)(!1), 2),
-                    Y = F[0],
-                    Q = F[1],
-                    G = a((0, t.useState)(!1), 2),
-                    W = G[0],
-                    H = G[1],
-                    Z = a((0, t.useState)(!1), 2),
-                    V = Z[0],
-                    q = Z[1],
-                    J = Xi("/portal_access_key"),
-                    K = la();
-                return B.error ? (0, Kr.jsx)(xi, {
-                    error: B.error,
+                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R, B, F, Y, Q, G, W, H, Z, V = ta(),
+                    q = Xi("/info"),
+                    J = a((0, t.useState)(!1), 2),
+                    K = J[0],
+                    X = J[1],
+                    $ = a((0, t.useState)(!1), 2),
+                    ee = $[0],
+                    te = $[1],
+                    ne = a((0, t.useState)(!1), 2),
+                    re = ne[0],
+                    oe = ne[1],
+                    ie = Xi("/portal_access_key"),
+                    ae = la();
+                return q.error ? (0, Kr.jsx)(xi, {
+                    error: q.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
                     children: [(0, Kr.jsxs)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Versions",
                         children: [(0, Kr.jsx)(Is, {
-                            name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
-                            value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
+                            name: null === (e = V.app) || void 0 === e ? void 0 : e.package,
+                            value: null === (n = V.versions) || void 0 === n ? void 0 : n.foursight,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
-                            github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
+                            github: At.IsFoursightFourfront(V) ? "4dn-dcic" : "dbmi-bgm",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "foursight-core",
-                            value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
+                            value: null === (r = V.versions) || void 0 === r ? void 0 : r.foursight_core,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "dcicutils",
-                            value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
+                            value: null === (o = V.versions) || void 0 === o ? void 0 : o.dcicutils,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "tibanna",
-                            value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
+                            value: null === (i = V.versions) || void 0 === i ? void 0 : i.tibanna,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "tibanna-ff",
-                            value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
+                            value: null === (s = V.versions) || void 0 === s ? void 0 : s.tibanna_ff,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "chalice",
-                            value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
+                            value: null === (u = V.versions) || void 0 === u ? void 0 : u.chalice,
                             monospace: !0,
                             copy: !0,
                             chalice: !0,
                             size: "2",
                             pypi: !0,
                             github: "aws"
                         }), (0, Kr.jsx)(Is, {
                             name: "python",
-                            value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
+                            value: null === (l = V.versions) || void 0 === l ? void 0 : l.python,
                             monospace: !0,
                             copy: !0,
                             python: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-server",
-                            value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
+                            value: (null === (c = V.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = q.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             elasticsearch: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch",
-                            value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
+                            value: null === (p = V.versions) || void 0 === p ? void 0 : p.elasticsearch,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-dsl",
-                            value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
+                            value: null === (h = V.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Credentials Info",
                         children: [(0, Kr.jsx)(Is, {
                             name: "AWS Account Number",
-                            value: B.get("app.credentials.aws_account_number"),
+                            value: q.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS Region Name",
-                            value: B.get("app.credentials.aws_region"),
+                            value: q.get("app.credentials.aws_region"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS User ARN",
-                            value: B.get("app.credentials.aws_user_arn"),
+                            value: q.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS Access Key ID",
-                            value: B.get("app.credentials.aws_access_key_id"),
+                            value: q.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(Is, {
+                        }), q.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(Is, {
                             name: "AWS S3 Access Key ID",
-                            value: B.get("environ.S3_AWS_ACCESS_KEY_ID"),
+                            value: q.get("environ.S3_AWS_ACCESS_KEY_ID"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Portal Access Key",
-                            value: J.get("key"),
+                            value: ie.get("key"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalAccessKey: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "Auth0 Client ID",
-                            value: B.get("app.credentials.auth0_client_id"),
+                            value: q.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Resources",
                         children: [(0, Kr.jsx)(Is, {
                             name: "Foursight Server",
-                            value: B.get("server.foursight"),
+                            value: q.get("server.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
-                            name: "Portal Server",
-                            value: B.get("server.portal"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            portalCertificate: !0
-                        }), (0, Kr.jsx)(Is, {
-                            name: "ElasticSearch Server",
-                            value: B.get("server.es"),
+                            name: "Foursight",
+                            value: null === (g = V.resources) || void 0 === g ? void 0 : g.foursight,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
-                            name: "RDS Server",
-                            value: B.get("server.rds"),
+                            name: "Portal",
+                            value: null === (y = V.resources) || void 0 === y ? void 0 : y.portal,
                             monospace: !0,
                             copy: !0,
-                            size: "2"
+                            size: "2",
+                            portalCertificate: !0
                         }), (0, Kr.jsx)(Is, {
-                            name: "SQS Server",
-                            value: B.get("server.sqs"),
+                            name: "ElasticSearch",
+                            value: null === (m = V.resources) || void 0 === m ? void 0 : m.es,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        })]
-                    }), (0, Kr.jsxs)(Ns, {
-                        info: B,
-                        title: "Environment Names",
-                        children: [(0, Kr.jsx)(Is, {
-                            name: "Environment Name",
-                            value: At.RegularName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Kr.jsx)(Is, {
-                            name: "Environment Name (Full)",
-                            value: At.FullName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Kr.jsx)(Is, {
-                            name: "Environment Name (Short)",
-                            value: At.ShortName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Kr.jsx)(Is, {
-                            name: "Environment Name (Public)",
-                            value: At.PublicName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
                         }), (0, Kr.jsx)(Is, {
-                            name: "Environment Name (Foursight)",
-                            value: At.FoursightName(At.Current(), R),
+                            name: "RDS",
+                            value: null === (v = V.resources) || void 0 === v ? void 0 : v.rds,
                             monospace: !0,
                             copy: !0,
-                            size: "3"
-                        }), (0, Kr.jsx)(Is, {
-                            name: "Environment Name (Preferred)",
-                            value: At.PreferredName(At.Current(R), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        })]
-                    }), (0, Kr.jsxs)(Ns, {
-                        info: B,
-                        title: "Bucket Names",
-                        children: [(0, Kr.jsx)(Is, {
-                            name: "Global Environment Bucket",
-                            value: B.get("buckets.env"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
+                            size: "2"
                         }), (0, Kr.jsx)(Is, {
-                            name: "Foursight Bucket Name",
-                            value: B.get("buckets.foursight"),
+                            name: "SQS",
+                            value: null === (M = V.resources) || void 0 === M ? void 0 : M.sqs,
                             monospace: !0,
                             copy: !0,
-                            size: "3"
+                            size: "2"
                         }), (0, Kr.jsx)(Is, {
-                            name: "Foursight Bucket Prefix",
-                            value: B.get("buckets.foursight_prefix"),
+                            name: "Redis",
+                            value: null === (b = V.resources) || void 0 === b ? void 0 : b.redis,
+                            nocheck: !(null !== (j = V.resources) && void 0 !== j && j.redis_running),
+                            check: null === (w = V.resources) || void 0 === w ? void 0 : w.redis_running,
                             monospace: !0,
                             copy: !0,
-                            size: "3"
+                            size: "2"
                         })]
-                    }), (0, Kr.jsx)(Ns, {
-                        info: B,
-                        title: "Environment & Bucket Names",
-                        children: (0, Kr.jsx)("pre", {
-                            className: "box",
-                            style: {
-                                border: "0",
-                                margin: "0",
-                                padding: "8",
-                                paddingBottom: "8",
-                                marginTop: "0"
-                            },
-                            children: (0, Kr.jsxs)("span", {
-                                children: [Bi.Format(B.get("buckets.info")), (null === (g = B.get("buckets.info")) || void 0 === g ? void 0 : g.length) > 1 ? (0, Kr.jsx)("div", {
-                                    style: {
-                                        height: "1px",
-                                        marginTop: "6px",
-                                        marginBottom: "6px",
-                                        background: "black"
-                                    }
-                                }) : (0, Kr.jsx)("span", {})]
-                            }, Dr()())
-                        })
-                    }), (0, Kr.jsx)(Ns, {
-                        info: B,
-                        title: "Ecosystem",
-                        show: !1,
-                        children: (0, Kr.jsx)("pre", {
-                            className: "box",
-                            style: {
-                                border: "0",
-                                margin: "0",
-                                paddingTop: "8",
-                                paddingBottom: "8",
-                                marginTop: "0"
-                            },
-                            children: Bi.Format(B.get("buckets.ecosystem"))
-                        })
                     }), (0, Kr.jsxs)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Authentication/Authorization Info",
-                        show: !1,
+                        show: !0,
                         children: [(0, Kr.jsx)(Is, {
                             name: "Email",
-                            value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
+                            value: null === (x = Br.Token()) || void 0 === x ? void 0 : x.user,
                             monospace: !0,
                             copy: !0,
-                            check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
-                            link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
+                            check: null === (N = Br.Token()) || void 0 === N ? void 0 : N.user_verified,
+                            link: kr.Path("/users/" + Br.LoggedInUser(V), !0),
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "First Name",
-                            value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
+                            value: null === (I = Br.Token()) || void 0 === I ? void 0 : I.first_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Last Name",
-                            value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
+                            value: null === (D = Br.Token()) || void 0 === D ? void 0 : D.last_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environments",
-                            value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
+                            value: null === (S = Br.Token()) || void 0 === S ? void 0 : S.allowed_envs.join(", "),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Audience",
-                            value: null === (j = Br.Token()) || void 0 === j ? void 0 : j.aud,
+                            value: null === (L = Br.Token()) || void 0 === L ? void 0 : L.aud,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Issued At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             value: (0, Kr.jsx)(ja.FormatDuration, {
-                                start: null === (w = Br.Token()) || void 0 === w ? void 0 : w.authenticated_at,
+                                start: null === (k = Br.Token()) || void 0 === k ? void 0 : k.authenticated_at,
                                 verbose: !0,
                                 fallback: "just now",
                                 suffix: "ago",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
                         }), (0, Kr.jsx)(Is, {
                             name: "Expires At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             value: (0, Kr.jsx)(ja.FormatDuration, {
-                                end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
+                                end: null === (C = Br.Token()) || void 0 === C ? void 0 : C.authenticated_until,
                                 verbose: !0,
                                 fallback: "now",
                                 suffix: "from now",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Using Redis",
+                            monospace: !0,
+                            size: "2",
+                            value: null !== (E = V.resources) && void 0 !== E && E.redis_running ? "Yes" : "No"
                         }), (0, Kr.jsx)("hr", {
                             style: {
                                 borderTop: "1px solid darkblue",
                                 marginTop: "8",
                                 marginBottom: "8"
                             }
-                        }), Y ? (0, Kr.jsxs)(Kr.Fragment, {
+                        }), K ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("small", {
                                 onClick: function() {
-                                    return Q(!1)
+                                    return X(!1)
                                 },
                                 style: {
                                     cursor: "pointer",
                                     color: "inherit"
                                 },
                                 children: (0, Kr.jsxs)("b", {
                                     children: [(0, Kr.jsx)("u", {
@@ -59854,109 +59784,209 @@
                                         cursor: "copy"
                                     }
                                 }), Bi.Format(Br.Token())]
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("small", {
                                 onClick: function() {
-                                    return Q(!0)
+                                    return X(!0)
                                 },
                                 style: {
                                     cursor: "pointer",
                                     color: "darkblue"
                                 },
                                 children: (0, Kr.jsxs)("b", {
                                     children: [(0, Kr.jsx)("u", {
                                         children: "AuthToken"
                                     }), "\xa0", Fr.UpArrow]
                                 })
                             }), (0, Kr.jsx)("br", {})]
                         })]
-                    }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
+                    }), (0, Kr.jsxs)(Ns, {
+                        info: q,
+                        title: "Environment Names",
+                        children: [(0, Kr.jsx)(Is, {
+                            name: "Environment Name",
+                            value: At.RegularName(At.Current(), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Environment Name (Full)",
+                            value: At.FullName(At.Current(), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Environment Name (Short)",
+                            value: At.ShortName(At.Current(), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Environment Name (Public)",
+                            value: At.PublicName(At.Current(), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Environment Name (Foursight)",
+                            value: At.FoursightName(At.Current(), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Environment Name (Preferred)",
+                            value: At.PreferredName(At.Current(V), V),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        })]
+                    }), (0, Kr.jsxs)(Ns, {
+                        info: q,
+                        title: "Bucket Names",
+                        children: [(0, Kr.jsx)(Is, {
+                            name: "Global Environment Bucket",
+                            value: q.get("buckets.env"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Foursight Bucket Name",
+                            value: q.get("buckets.foursight"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Kr.jsx)(Is, {
+                            name: "Foursight Bucket Prefix",
+                            value: q.get("buckets.foursight_prefix"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        })]
+                    }), (0, Kr.jsx)(Ns, {
+                        info: q,
+                        title: "Environment & Bucket Names",
+                        children: (0, Kr.jsx)("pre", {
+                            className: "box",
+                            style: {
+                                border: "0",
+                                margin: "0",
+                                padding: "8",
+                                paddingBottom: "8",
+                                marginTop: "0"
+                            },
+                            children: (0, Kr.jsxs)("span", {
+                                children: [Bi.Format(q.get("buckets.info")), (null === (_ = q.get("buckets.info")) || void 0 === _ ? void 0 : _.length) > 1 ? (0, Kr.jsx)("div", {
+                                    style: {
+                                        height: "1px",
+                                        marginTop: "6px",
+                                        marginBottom: "6px",
+                                        background: "black"
+                                    }
+                                }) : (0, Kr.jsx)("span", {})]
+                            }, Dr()())
+                        })
+                    }), (0, Kr.jsx)(Ns, {
+                        info: q,
+                        title: "Ecosystem",
+                        show: !1,
+                        children: (0, Kr.jsx)("pre", {
+                            className: "box",
+                            style: {
+                                border: "0",
+                                margin: "0",
+                                paddingTop: "8",
+                                paddingBottom: "8",
+                                marginTop: "0"
+                            },
+                            children: Bi.Format(q.get("buckets.ecosystem"))
+                        })
+                    }), q.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && q.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsxs)(Ns, {
-                            info: B,
+                            info: q,
                             title: "Logs",
                             children: [(0, Kr.jsx)(Is, {
                                 name: "Log Group",
-                                value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
+                                value: q.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                 monospace: !0,
                                 size: "2"
                             }), (0, Kr.jsx)(Is, {
                                 name: "Log Stream",
-                                value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
+                                value: q.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                 monospace: !0,
                                 size: "2"
                             })]
                         })
-                    }), B.get("app.lambda") && (0, Kr.jsxs)(Ns, {
-                        info: B,
+                    }), q.get("app.lambda") && (0, Kr.jsxs)(Ns, {
+                        info: q,
                         title: "Lambda",
                         show: !1,
                         children: [(0, Kr.jsx)(Is, {
                             name: "Name",
-                            value: B.get("app.lambda.lambda_name"),
+                            value: q.get("app.lambda.lambda_name"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Function",
-                            value: B.get("app.lambda.lambda_function_name"),
+                            value: q.get("app.lambda.lambda_function_name"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "ARN",
-                            value: B.get("app.lambda.lambda_function_arn"),
+                            value: q.get("app.lambda.lambda_function_arn"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "S3 Location",
-                            value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
+                            value: q.get("app.lambda.lambda_code_s3_bucket") + "/" + q.get("app.lambda.lambda_code_s3_bucket_key"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Size",
-                            value: B.get("app.lambda.lambda_code_size"),
+                            value: q.get("app.lambda.lambda_code_size"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Modified",
-                            value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
+                            value: Pr.FormatDateTime(q.get("app.lambda.lambda_modified")),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Role",
-                            value: B.get("app.lambda.lambda_role"),
+                            value: q.get("app.lambda.lambda_role"),
                             monospace: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Miscellany",
-                        children: [V ? (0, Kr.jsxs)(Kr.Fragment, {
+                        children: [re ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 id: "tooltip-info-reloading",
                                 style: {
                                     float: "right"
                                 },
                                 children: (0, Kr.jsx)(no, {
-                                    condition: V,
+                                    condition: re,
                                     label: "",
                                     color: "darkblue"
                                 })
                             }), (0, Kr.jsx)(Mi, {
                                 id: "tooltip-info-reloading",
                                 position: "bottom",
                                 size: "small",
                                 text: "Reloading the Foursight app."
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
-                                    return q(!0), void K("/__reloadlambda__", {
+                                    return oe(!0), void ae("/__reloadlambda__", {
                                         onDone: function() {
-                                            return q(!1)
+                                            return oe(!1)
                                         }
                                     })
                                 },
                                 id: "tooltip-info-reload",
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
@@ -59977,72 +60007,72 @@
                                 cursor: "pointer"
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("img", {
                                 alt: "Clear Cache",
                                 src: Ut.ClearCache(),
                                 height: "19",
                                 onClick: function() {
-                                    K(zt.Url("/__functioncacheclear__", !1))
+                                    ae(zt.Url("/__functioncacheclear__", !1))
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
                         }), (0, Kr.jsx)(Is, {
                             name: "App Deployed At",
-                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
+                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (T = V.app) || void 0 === T ? void 0 : T.deployed) + Pr.FormatDuration(null === (A = V.app) || void 0 === A ? void 0 : A.deployed, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             copy: !0,
                             optional: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "App Launched At",
-                            value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
+                            value: (null === (O = V.app) || void 0 === O ? void 0 : O.launched) + Pr.FormatDuration(null === (z = V.app) || void 0 === z ? void 0 : z.launched, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Page Loaded At",
-                            value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
+                            value: q.get("page.loaded") + Pr.FormatDuration(q.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Package",
-                            value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
+                            value: null === (U = V.app) || void 0 === U ? void 0 : U.package,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Stage",
-                            value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
+                            value: null === (P = V.app) || void 0 === P ? void 0 : P.stage,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment",
                             value: At.Current(),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Domain",
-                            value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
+                            value: null === (R = V.app) || void 0 === R ? void 0 : R.domain,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Context",
-                            value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
+                            value: null === (B = V.app) || void 0 === B ? void 0 : B.context,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Path",
-                            value: B.get("page.path"),
+                            value: q.get("page.path"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Endpoint",
-                            value: B.get("page.endpoint"),
+                            value: q.get("page.endpoint"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Client (React UI)",
                             value: kr.BaseUrl(),
                             monospace: !0,
                             size: "2"
@@ -60050,85 +60080,85 @@
                             name: "Server (React API)",
                             value: zt.BaseUrl(),
                             monospace: !0,
                             size: "2",
                             apiCache: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "Checks File",
-                            value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
+                            value: null === (F = q.data) || void 0 === F || null === (Y = F.checks) || void 0 === Y ? void 0 : Y.file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(Is, {
+                        }), (null === (Q = V.app) || void 0 === Q ? void 0 : Q.accounts_file) && (0, Kr.jsx)(Is, {
                             name: "Accounts File",
-                            value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
+                            value: null === (G = V.app) || void 0 === G ? void 0 : G.accounts_file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(Is, {
+                        }), (null === (W = V.app) || void 0 === W ? void 0 : W.accounts_file_from_s3) && (0, Kr.jsx)(Is, {
                             name: "Accounts File (S3)",
-                            value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
+                            value: null === (H = V.app) || void 0 === H ? void 0 : H.accounts_file_from_s3,
                             monospace: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsx)(Ns, {
-                        info: B,
-                        title: "GAC: ".concat(B.get("gac.name")),
+                        info: q,
+                        title: "GAC: ".concat(q.get("gac.name")),
                         show: !1,
-                        children: B.get("gac.values") ? (0, Kr.jsx)("span", {
-                            children: Object.keys(B.get("gac.values")).map((function(e) {
+                        children: q.get("gac.values") ? (0, Kr.jsx)("span", {
+                            children: Object.keys(q.get("gac.values")).map((function(e) {
                                 return (0, Kr.jsx)(Is, {
                                     name: e,
-                                    value: B.get("gac.values")[e],
+                                    value: q.get("gac.values")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
                     }), (0, Kr.jsx)(Ns, {
-                        info: B,
+                        info: q,
                         title: "Environment Variables",
                         show: !1,
-                        children: B.get("environ") ? (0, Kr.jsx)("span", {
-                            children: Object.keys(B.get("environ")).map((function(e) {
+                        children: q.get("environ") ? (0, Kr.jsx)("span", {
+                            children: Object.keys(q.get("environ")).map((function(e) {
                                 return (0, Kr.jsx)(Is, {
                                     name: e,
-                                    value: B.get("environ")[e],
+                                    value: q.get("environ")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
-                    }), (null === (P = R.app) || void 0 === P ? void 0 : P.accounts) && (0, Kr.jsx)("div", {
+                    }), (null === (Z = V.app) || void 0 === Z ? void 0 : Z.accounts) && (0, Kr.jsx)("div", {
                         className: "container",
                         style: {
                             marginTop: "4pt"
                         },
-                        children: W ? (0, Kr.jsx)(Kr.Fragment, {
+                        children: ee ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsx)(sa, {})
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
-                                    return H(!0)
+                                    return te(!0)
                                 },
                                 style: {
                                     cursor: "pointer"
                                 },
                                 children: "Show Accounts"
                             }), (0, Kr.jsxs)("div", {
                                 className: "box",
                                 children: ["Click ", (0, Kr.jsx)("b", {
                                     onClick: function() {
-                                        return H(!0)
+                                        return te(!0)
                                     },
                                     style: {
                                         cursor: "pointer"
                                     },
                                     children: "here"
                                 }), " to ", (0, Kr.jsx)("span", {
                                     onClick: function() {
-                                        return H(!0)
+                                        return te(!0)
                                     },
                                     style: {
                                         cursor: "pointer"
                                     },
                                     children: "show"
                                 }), "."]
                             })]
```

### Comparing `foursight_core-4.2.0.1b2/foursight_core/route_prefixes.py` & `foursight_core-4.2.0.1b3/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/routes.py` & `foursight_core-4.2.0.1b3/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/run_result.py` & `foursight_core-4.2.0.1b3/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/s3_connection.py` & `foursight_core-4.2.0.1b3/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/schedule_decorator.py` & `foursight_core-4.2.0.1b3/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.2.0.1b3/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.2.0.1b3/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/sqs_utils.py` & `foursight_core-4.2.0.1b3/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/stage.py` & `foursight_core-4.2.0.1b3/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/base.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/header.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/history.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/info.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/unused.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/user.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/users.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/view_checks.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/foursight_core/templates/view_groups.html` & `foursight_core-4.2.0.1b3/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b2/pyproject.toml` & `foursight_core-4.2.0.1b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.2.0.1b2"  # to become 4.2.0
+version = "4.2.0.1b3"  # to become 4.2.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.2.0.1b2/setup.py` & `foursight_core-4.2.0.1b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-core',
-    'version': '4.2.0.1b2',
+    'version': '4.2.0.1b3',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_core-4.2.0.1b2/PKG-INFO` & `foursight_core-4.2.0.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.2.0.1b2
+Version: 4.2.0.1b3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

