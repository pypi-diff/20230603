# Comparing `tmp/sonatype_nxrm_sdk-0.1.4.tar.gz` & `tmp/sonatype_nxrm_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatype_nxrm_sdk-0.1.4.tar", max compression
+gzip compressed data, was "sonatype_nxrm_sdk-0.1.5.tar", max compression
```

## Comparing `sonatype_nxrm_sdk-0.1.4.tar` & `sonatype_nxrm_sdk-0.1.5.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0     1070 2023-06-03 14:33:29.644137 sonatype_nxrm_sdk-0.1.4/LICENSE
--rw-r--r--   0        0        0     3061 2023-06-03 14:33:29.644137 sonatype_nxrm_sdk-0.1.4/README.md
--rw-r--r--   0        0        0    15893 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/__init__.py
--rw-r--r--   0        0        0     2270 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/__init__.py
--rw-r--r--   0        0        0    11638 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/assets_api.py
--rw-r--r--   0        0        0     4131 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/azure_blob_store_api.py
--rw-r--r--   0        0        0    59097 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/blob_store_api.py
--rw-r--r--   0        0        0    26117 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/components_api.py
--rw-r--r--   0        0        0    18303 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/content_selectors_api.py
--rw-r--r--   0        0        0    14563 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/email_api.py
--rw-r--r--   0        0        0     7398 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/formats_api.py
--rw-r--r--   0        0        0    10230 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/lifecycle_api.py
--rw-r--r--   0        0        0    15312 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/manage_iq_server_configuration_api.py
--rw-r--r--   0        0        0    10243 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/product_licensing_api.py
--rw-r--r--   0        0        0    12528 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/read_only_api.py
--rw-r--r--   0        0        0    23718 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/replication_api.py
--rw-r--r--   0        0        0   485097 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/repository_management_api.py
--rw-r--r--   0        0        0    18744 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/routing_rules_api.py
--rw-r--r--   0        0        0    20687 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/script_api.py
--rw-r--r--   0        0        0    43673 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/search_api.py
--rw-r--r--   0        0        0    13152 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_atlassian_crowd_api.py
--rw-r--r--   0        0        0    15331 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_certificates_api.py
--rw-r--r--   0        0        0     7197 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_anonymous_access_api.py
--rw-r--r--   0        0        0     3926 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_api.py
--rw-r--r--   0        0        0     3752 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_jwt_api.py
--rw-r--r--   0        0        0    20724 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_ldap_api.py
--rw-r--r--   0        0        0    56088 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_privileges_api.py
--rw-r--r--   0        0        0    10206 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_realms_api.py
--rw-r--r--   0        0        0    18811 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_roles_api.py
--rw-r--r--   0        0        0    15886 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_saml_api.py
--rw-r--r--   0        0        0    10300 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_user_tokens_api.py
--rw-r--r--   0        0        0    23276 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_users_api.py
--rw-r--r--   0        0        0    26090 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/staging_api.py
--rw-r--r--   0        0        0     9859 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/status_api.py
--rw-r--r--   0        0        0     7471 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/support_api.py
--rw-r--r--   0        0        0    43981 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/tags_api.py
--rw-r--r--   0        0        0    13751 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/tasks_api.py
--rw-r--r--   0        0        0    24417 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api_client.py
--rw-r--r--   0        0        0     7997 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/configuration.py
--rw-r--r--   0        0        0    13568 2023-06-03 14:33:29.652137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/__init__.py
--rw-r--r--   0        0        0     6776 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/abstract_api_repository.py
--rw-r--r--   0        0        0     5097 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/anonymous_access_settings_xo.py
--rw-r--r--   0        0        0    12234 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_certificate.py
--rw-r--r--   0        0        0     8697 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_create_user.py
--rw-r--r--   0        0        0    13496 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_email_configuration.py
--rw-r--r--   0        0        0     3811 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_email_validation.py
--rw-r--r--   0        0        0     9671 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_license_details_xo.py
--rw-r--r--   0        0        0     5840 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege.py
--rw-r--r--   0        0        0     7136 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_application_request.py
--rw-r--r--   0        0        0     7935 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_admin_request.py
--rw-r--r--   0        0        0     9404 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_content_selector_request.py
--rw-r--r--   0        0        0     7911 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_view_request.py
--rw-r--r--   0        0        0     6757 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_script_request.py
--rw-r--r--   0        0        0     4971 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_wildcard_request.py
--rw-r--r--   0        0        0    10674 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_user.py
--rw-r--r--   0        0        0     3608 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_user_source.py
--rw-r--r--   0        0        0     8410 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_api_repository.py
--rw-r--r--   0        0        0     3475 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_repositories_attributes.py
--rw-r--r--   0        0        0     8747 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11198 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_api_repository.py
--rw-r--r--   0        0        0     4324 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_repositories_attributes.py
--rw-r--r--   0        0        0    11362 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_repository_api_request.py
--rw-r--r--   0        0        0     4378 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_signing_repositories_attributes.py
--rw-r--r--   0        0        0    10609 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/asset_xo.py
--rw-r--r--   0        0        0     5126 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_authentication.py
--rw-r--r--   0        0        0     5994 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_bucket_configuration.py
--rw-r--r--   0        0        0     5378 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_model.py
--rw-r--r--   0        0        0     5819 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_connection_xo.py
--rw-r--r--   0        0        0     3213 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/base_tag_xo.py
--rw-r--r--   0        0        0     4326 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/blob_store_api_soft_quota.py
--rw-r--r--   0        0        0     4842 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/blob_store_quota_result_xo.py
--rw-r--r--   0        0        0     3741 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_attributes.py
--rw-r--r--   0        0        0     6123 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_group_repository_api_request.py
--rw-r--r--   0        0        0     6926 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11169 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_proxy_api_repository.py
--rw-r--r--   0        0        0    11333 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_proxy_repository_api_request.py
--rw-r--r--   0        0        0     3516 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/cleanup_policy_attributes.py
--rw-r--r--   0        0        0    10780 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/cocoapods_proxy_repository_api_request.py
--rw-r--r--   0        0        0     3771 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/component_attributes.py
--rw-r--r--   0        0        0     6876 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/component_xo.py
--rw-r--r--   0        0        0    10620 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/conan_proxy_repository_api_request.py
--rw-r--r--   0        0        0    10620 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/conda_proxy_repository_api_request.py
--rw-r--r--   0        0        0     5180 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_create_request.py
--rw-r--r--   0        0        0     6211 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_response.py
--rw-r--r--   0        0        0     4390 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_update_request.py
--rw-r--r--   0        0        0    35709 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/create_ldap_server_xo.py
--rw-r--r--   0        0        0     8013 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/crowd_api_xo.py
--rw-r--r--   0        0        0     7239 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_attributes.py
--rw-r--r--   0        0        0     6741 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_group_api_repository.py
--rw-r--r--   0        0        0     7022 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_group_repository_api_request.py
--rw-r--r--   0        0        0     7541 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_api_repository.py
--rw-r--r--   0        0        0     7868 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_repository_api_request.py
--rw-r--r--   0        0        0     7652 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_storage_attributes.py
--rw-r--r--   0        0        0    12318 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_api_repository.py
--rw-r--r--   0        0        0     6977 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_attributes.py
--rw-r--r--   0        0        0    12510 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_repository_api_request.py
--rw-r--r--   0        0        0     5099 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_create_request.py
--rw-r--r--   0        0        0     4343 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_model.py
--rw-r--r--   0        0        0     4439 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_update_request.py
--rw-r--r--   0        0        0     8247 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/generic_blob_store_api_response.py
--rw-r--r--   0        0        0     6950 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/git_lfs_hosted_repository_api_request.py
--rw-r--r--   0        0        0     6143 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/golang_group_repository_api_request.py
--rw-r--r--   0        0        0    10660 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/golang_proxy_repository_api_request.py
--rw-r--r--   0        0        0     3374 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_attributes.py
--rw-r--r--   0        0        0     6096 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_create_request.py
--rw-r--r--   0        0        0     5305 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_model.py
--rw-r--r--   0        0        0     5996 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_response.py
--rw-r--r--   0        0        0     5433 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_update_request.py
--rw-r--r--   0        0        0     4442 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_deploy_attributes.py
--rw-r--r--   0        0        0     6902 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/helm_hosted_repository_api_request.py
--rw-r--r--   0        0        0    10580 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/helm_proxy_repository_api_request.py
--rw-r--r--   0        0        0     6477 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/hosted_storage_attributes.py
--rw-r--r--   0        0        0     6350 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_attributes.py
--rw-r--r--   0        0        0     6752 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_attributes_with_preemptive_auth.py
--rw-r--r--   0        0        0     8905 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_attributes.py
--rw-r--r--   0        0        0     6970 2023-06-03 14:33:29.656137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_authentication_attributes.py
--rw-r--r--   0        0        0     8465 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_authentication_attributes_with_preemptive.py
--rw-r--r--   0        0        0     2514 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/input_stream.py
--rw-r--r--   0        0        0     3907 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/iq_connection_verification_xo.py
--rw-r--r--   0        0        0    11003 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/iq_connection_xo.py
--rw-r--r--   0        0        0     6395 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_attributes.py
--rw-r--r--   0        0        0     6123 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_group_repository_api_request.py
--rw-r--r--   0        0        0     7489 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_hosted_api_repository.py
--rw-r--r--   0        0        0     7798 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11283 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_proxy_api_repository.py
--rw-r--r--   0        0        0    11501 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_proxy_repository_api_request.py
--rw-r--r--   0        0        0     4636 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/negative_cache_attributes.py
--rw-r--r--   0        0        0     4748 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_attributes.py
--rw-r--r--   0        0        0     6101 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_group_repository_api_request.py
--rw-r--r--   0        0        0     6878 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11035 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_proxy_api_repository.py
--rw-r--r--   0        0        0    11199 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_proxy_repository_api_request.py
--rw-r--r--   0        0        0     4862 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_attributes.py
--rw-r--r--   0        0        0     6123 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_group_repository_api_request.py
--rw-r--r--   0        0        0     6926 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11408 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_proxy_api_repository.py
--rw-r--r--   0        0        0    11572 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_proxy_repository_api_request.py
--rw-r--r--   0        0        0    10500 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/p2_proxy_repository_api_request.py
--rw-r--r--   0        0        0     3866 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page.py
--rw-r--r--   0        0        0     3953 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_asset_xo.py
--rw-r--r--   0        0        0     4013 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_component_xo.py
--rw-r--r--   0        0        0     3923 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_tag_xo.py
--rw-r--r--   0        0        0     3938 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_task_xo.py
--rw-r--r--   0        0        0     5695 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/proxy_attributes.py
--rw-r--r--   0        0        0     6103 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_group_repository_api_request.py
--rw-r--r--   0        0        0     6902 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_hosted_repository_api_request.py
--rw-r--r--   0        0        0    10580 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_proxy_repository_api_request.py
--rw-r--r--   0        0        0     6043 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_group_repository_api_request.py
--rw-r--r--   0        0        0     6830 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_hosted_repository_api_request.py
--rw-r--r--   0        0        0    10460 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_proxy_repository_api_request.py
--rw-r--r--   0        0        0     3808 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_attributes.py
--rw-r--r--   0        0        0     6748 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_group_repository_api_request.py
--rw-r--r--   0        0        0     7582 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11199 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_proxy_repository_api_request.py
--rw-r--r--   0        0        0    35823 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/read_ldap_server_xo.py
--rw-r--r--   0        0        0     4773 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/read_only_state.py
--rw-r--r--   0        0        0     3572 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/realm_api_xo.py
--rw-r--r--   0        0        0     4532 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_attributes.py
--rw-r--r--   0        0        0    13735 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_connection_xo.py
--rw-r--r--   0        0        0     6262 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_enable_xo.py
--rw-r--r--   0        0        0     5609 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/repository_xo.py
--rw-r--r--   0        0        0     6889 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/result.py
--rw-r--r--   0        0        0     6265 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/role_xo_request.py
--rw-r--r--   0        0        0     8038 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/role_xo_response.py
--rw-r--r--   0        0        0     5863 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/routing_rule_xo.py
--rw-r--r--   0        0        0     6183 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_group_repository_api_request.py
--rw-r--r--   0        0        0     6998 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_hosted_repository_api_request.py
--rw-r--r--   0        0        0    10740 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7150 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_advanced_bucket_connection.py
--rw-r--r--   0        0        0     6209 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket.py
--rw-r--r--   0        0        0     6529 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket_configuration.py
--rw-r--r--   0        0        0     6543 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket_security.py
--rw-r--r--   0        0        0     4794 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_encryption.py
--rw-r--r--   0        0        0     6006 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_model.py
--rw-r--r--   0        0        0    12177 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/saml_configuration_xo.py
--rw-r--r--   0        0        0     3700 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/script_result_xo.py
--rw-r--r--   0        0        0     4193 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/script_xo.py
--rw-r--r--   0        0        0     6028 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_group_deploy_repository.py
--rw-r--r--   0        0        0     5890 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_group_repository.py
--rw-r--r--   0        0        0     6669 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_hosted_repository.py
--rw-r--r--   0        0        0    10524 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_proxy_repository.py
--rw-r--r--   0        0        0     6266 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/stack_trace_element.py
--rw-r--r--   0        0        0     4962 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/storage_attributes.py
--rw-r--r--   0        0        0    11779 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/support_zip_generator_request.py
--rw-r--r--   0        0        0     4900 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/support_zip_xo.py
--rw-r--r--   0        0        0     5353 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/tag_xo.py
--rw-r--r--   0        0        0     7612 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/task_xo.py
--rw-r--r--   0        0        0     6108 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/throwable.py
--rw-r--r--   0        0        0    36352 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/update_ldap_server_xo.py
--rw-r--r--   0        0        0     5819 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/upload_definition_xo.py
--rw-r--r--   0        0        0     5934 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/upload_field_definition_xo.py
--rw-r--r--   0        0        0     4299 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/user_tokens_api_model.py
--rw-r--r--   0        0        0    40587 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/v1_components_body.py
--rw-r--r--   0        0        0     4795 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_attributes.py
--rw-r--r--   0        0        0     6964 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_group_repository_api_request.py
--rw-r--r--   0        0        0     7385 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_hosted_api_repository.py
--rw-r--r--   0        0        0     7694 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_hosted_repository_api_request.py
--rw-r--r--   0        0        0    11415 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_proxy_repository_api_request.py
--rw-r--r--   0        0        0     4378 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_signing_repositories_attributes.py
--rw-r--r--   0        0        0    13274 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/nxrm_sdk/rest.py
--rw-r--r--   0        0        0      629 2023-06-03 14:33:29.660137 sonatype_nxrm_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 sonatype_nxrm_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 15:00:29.762599 sonatype_nxrm_sdk-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3061 2023-06-03 15:00:29.762599 sonatype_nxrm_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0    15893 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/__init__.py
+-rw-r--r--   0        0        0     2270 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/__init__.py
+-rw-r--r--   0        0        0    11638 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/assets_api.py
+-rw-r--r--   0        0        0     4131 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/azure_blob_store_api.py
+-rw-r--r--   0        0        0    59097 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/blob_store_api.py
+-rw-r--r--   0        0        0    26117 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/components_api.py
+-rw-r--r--   0        0        0    18303 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/content_selectors_api.py
+-rw-r--r--   0        0        0    14563 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/email_api.py
+-rw-r--r--   0        0        0     7398 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/formats_api.py
+-rw-r--r--   0        0        0    10230 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/lifecycle_api.py
+-rw-r--r--   0        0        0    15312 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/manage_iq_server_configuration_api.py
+-rw-r--r--   0        0        0    10243 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/product_licensing_api.py
+-rw-r--r--   0        0        0    12528 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/read_only_api.py
+-rw-r--r--   0        0        0    23718 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/replication_api.py
+-rw-r--r--   0        0        0   485097 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/repository_management_api.py
+-rw-r--r--   0        0        0    18744 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/routing_rules_api.py
+-rw-r--r--   0        0        0    20687 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/script_api.py
+-rw-r--r--   0        0        0    43673 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/search_api.py
+-rw-r--r--   0        0        0    13152 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_atlassian_crowd_api.py
+-rw-r--r--   0        0        0    15331 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_certificates_api.py
+-rw-r--r--   0        0        0     7197 2023-06-03 15:00:29.770599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_anonymous_access_api.py
+-rw-r--r--   0        0        0     3926 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_api.py
+-rw-r--r--   0        0        0     3752 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_jwt_api.py
+-rw-r--r--   0        0        0    20724 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_ldap_api.py
+-rw-r--r--   0        0        0    56088 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_privileges_api.py
+-rw-r--r--   0        0        0    10206 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_realms_api.py
+-rw-r--r--   0        0        0    18811 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_roles_api.py
+-rw-r--r--   0        0        0    15886 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_saml_api.py
+-rw-r--r--   0        0        0    10300 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_user_tokens_api.py
+-rw-r--r--   0        0        0    23276 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_users_api.py
+-rw-r--r--   0        0        0    26090 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/staging_api.py
+-rw-r--r--   0        0        0     9859 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/status_api.py
+-rw-r--r--   0        0        0     7471 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/support_api.py
+-rw-r--r--   0        0        0    43981 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/tags_api.py
+-rw-r--r--   0        0        0    13751 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/tasks_api.py
+-rw-r--r--   0        0        0    24417 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api_client.py
+-rw-r--r--   0        0        0     7997 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/configuration.py
+-rw-r--r--   0        0        0    13568 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/__init__.py
+-rw-r--r--   0        0        0     6776 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/abstract_api_repository.py
+-rw-r--r--   0        0        0     5097 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/anonymous_access_settings_xo.py
+-rw-r--r--   0        0        0    12234 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_certificate.py
+-rw-r--r--   0        0        0     8697 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_create_user.py
+-rw-r--r--   0        0        0    13496 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_email_configuration.py
+-rw-r--r--   0        0        0     3811 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_email_validation.py
+-rw-r--r--   0        0        0     9671 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_license_details_xo.py
+-rw-r--r--   0        0        0     5840 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege.py
+-rw-r--r--   0        0        0     7136 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_application_request.py
+-rw-r--r--   0        0        0     7935 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_admin_request.py
+-rw-r--r--   0        0        0     9404 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_content_selector_request.py
+-rw-r--r--   0        0        0     7911 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_view_request.py
+-rw-r--r--   0        0        0     6757 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_script_request.py
+-rw-r--r--   0        0        0     4971 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_wildcard_request.py
+-rw-r--r--   0        0        0    10674 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_user.py
+-rw-r--r--   0        0        0     3608 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_user_source.py
+-rw-r--r--   0        0        0     8410 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_api_repository.py
+-rw-r--r--   0        0        0     3475 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_repositories_attributes.py
+-rw-r--r--   0        0        0     8747 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11198 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_api_repository.py
+-rw-r--r--   0        0        0     4324 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_repositories_attributes.py
+-rw-r--r--   0        0        0    11362 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     4378 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_signing_repositories_attributes.py
+-rw-r--r--   0        0        0    10609 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/asset_xo.py
+-rw-r--r--   0        0        0     5126 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_authentication.py
+-rw-r--r--   0        0        0     5994 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_bucket_configuration.py
+-rw-r--r--   0        0        0     5378 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_model.py
+-rw-r--r--   0        0        0     5819 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_connection_xo.py
+-rw-r--r--   0        0        0     3213 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/base_tag_xo.py
+-rw-r--r--   0        0        0     4326 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/blob_store_api_soft_quota.py
+-rw-r--r--   0        0        0     4842 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/blob_store_quota_result_xo.py
+-rw-r--r--   0        0        0     3741 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_attributes.py
+-rw-r--r--   0        0        0     6123 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_group_repository_api_request.py
+-rw-r--r--   0        0        0     6926 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11169 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_proxy_api_repository.py
+-rw-r--r--   0        0        0    11333 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     3516 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/cleanup_policy_attributes.py
+-rw-r--r--   0        0        0    10780 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/cocoapods_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     3771 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/component_attributes.py
+-rw-r--r--   0        0        0     6876 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/component_xo.py
+-rw-r--r--   0        0        0    10620 2023-06-03 15:00:29.774599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/conan_proxy_repository_api_request.py
+-rw-r--r--   0        0        0    10620 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/conda_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     5180 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_create_request.py
+-rw-r--r--   0        0        0     6211 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_response.py
+-rw-r--r--   0        0        0     4390 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_update_request.py
+-rw-r--r--   0        0        0    35709 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/create_ldap_server_xo.py
+-rw-r--r--   0        0        0     8013 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/crowd_api_xo.py
+-rw-r--r--   0        0        0     7239 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_attributes.py
+-rw-r--r--   0        0        0     6741 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_group_api_repository.py
+-rw-r--r--   0        0        0     7022 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_group_repository_api_request.py
+-rw-r--r--   0        0        0     7541 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_api_repository.py
+-rw-r--r--   0        0        0     7868 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     7652 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_storage_attributes.py
+-rw-r--r--   0        0        0    12318 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_api_repository.py
+-rw-r--r--   0        0        0     6977 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_attributes.py
+-rw-r--r--   0        0        0    12510 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     5099 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_create_request.py
+-rw-r--r--   0        0        0     4343 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_model.py
+-rw-r--r--   0        0        0     4439 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_update_request.py
+-rw-r--r--   0        0        0     8247 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/generic_blob_store_api_response.py
+-rw-r--r--   0        0        0     6950 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/git_lfs_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     6143 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/golang_group_repository_api_request.py
+-rw-r--r--   0        0        0    10660 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/golang_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     3374 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_attributes.py
+-rw-r--r--   0        0        0     6096 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_create_request.py
+-rw-r--r--   0        0        0     5305 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_model.py
+-rw-r--r--   0        0        0     5996 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_response.py
+-rw-r--r--   0        0        0     5433 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_update_request.py
+-rw-r--r--   0        0        0     4442 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_deploy_attributes.py
+-rw-r--r--   0        0        0     6902 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/helm_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    10580 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/helm_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     6477 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/hosted_storage_attributes.py
+-rw-r--r--   0        0        0     6350 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_attributes.py
+-rw-r--r--   0        0        0     6752 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_attributes_with_preemptive_auth.py
+-rw-r--r--   0        0        0     8905 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_attributes.py
+-rw-r--r--   0        0        0     6970 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_authentication_attributes.py
+-rw-r--r--   0        0        0     8465 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_authentication_attributes_with_preemptive.py
+-rw-r--r--   0        0        0     2514 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/input_stream.py
+-rw-r--r--   0        0        0     3907 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/iq_connection_verification_xo.py
+-rw-r--r--   0        0        0    11003 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/iq_connection_xo.py
+-rw-r--r--   0        0        0     6395 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_attributes.py
+-rw-r--r--   0        0        0     6123 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_group_repository_api_request.py
+-rw-r--r--   0        0        0     7489 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_hosted_api_repository.py
+-rw-r--r--   0        0        0     7798 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11283 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_proxy_api_repository.py
+-rw-r--r--   0        0        0    11501 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     4636 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/negative_cache_attributes.py
+-rw-r--r--   0        0        0     4748 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_attributes.py
+-rw-r--r--   0        0        0     6101 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_group_repository_api_request.py
+-rw-r--r--   0        0        0     6878 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11035 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_proxy_api_repository.py
+-rw-r--r--   0        0        0    11199 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     4862 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_attributes.py
+-rw-r--r--   0        0        0     6123 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_group_repository_api_request.py
+-rw-r--r--   0        0        0     6926 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11408 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_proxy_api_repository.py
+-rw-r--r--   0        0        0    11572 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_proxy_repository_api_request.py
+-rw-r--r--   0        0        0    10500 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/p2_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     3866 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page.py
+-rw-r--r--   0        0        0     3953 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_asset_xo.py
+-rw-r--r--   0        0        0     4013 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_component_xo.py
+-rw-r--r--   0        0        0     3923 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_tag_xo.py
+-rw-r--r--   0        0        0     3938 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_task_xo.py
+-rw-r--r--   0        0        0     5695 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/proxy_attributes.py
+-rw-r--r--   0        0        0     6103 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_group_repository_api_request.py
+-rw-r--r--   0        0        0     6902 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    10580 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     6043 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_group_repository_api_request.py
+-rw-r--r--   0        0        0     6830 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    10460 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     3808 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_attributes.py
+-rw-r--r--   0        0        0     6748 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_group_repository_api_request.py
+-rw-r--r--   0        0        0     7582 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11199 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_proxy_repository_api_request.py
+-rw-r--r--   0        0        0    35823 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/read_ldap_server_xo.py
+-rw-r--r--   0        0        0     4773 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/read_only_state.py
+-rw-r--r--   0        0        0     3572 2023-06-03 15:00:29.778599 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/realm_api_xo.py
+-rw-r--r--   0        0        0     4532 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_attributes.py
+-rw-r--r--   0        0        0    13735 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_connection_xo.py
+-rw-r--r--   0        0        0     6262 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_enable_xo.py
+-rw-r--r--   0        0        0     5609 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/repository_xo.py
+-rw-r--r--   0        0        0     6889 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/result.py
+-rw-r--r--   0        0        0     6265 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/role_xo_request.py
+-rw-r--r--   0        0        0     8038 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/role_xo_response.py
+-rw-r--r--   0        0        0     5863 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/routing_rule_xo.py
+-rw-r--r--   0        0        0     6183 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_group_repository_api_request.py
+-rw-r--r--   0        0        0     6998 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    10740 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7150 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_advanced_bucket_connection.py
+-rw-r--r--   0        0        0     6209 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket.py
+-rw-r--r--   0        0        0     6529 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket_configuration.py
+-rw-r--r--   0        0        0     6543 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket_security.py
+-rw-r--r--   0        0        0     4794 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_encryption.py
+-rw-r--r--   0        0        0     6006 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_model.py
+-rw-r--r--   0        0        0    12177 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/saml_configuration_xo.py
+-rw-r--r--   0        0        0     3700 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/script_result_xo.py
+-rw-r--r--   0        0        0     4193 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/script_xo.py
+-rw-r--r--   0        0        0     6028 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_group_deploy_repository.py
+-rw-r--r--   0        0        0     5890 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_group_repository.py
+-rw-r--r--   0        0        0     6669 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_hosted_repository.py
+-rw-r--r--   0        0        0    10524 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_proxy_repository.py
+-rw-r--r--   0        0        0     6266 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/stack_trace_element.py
+-rw-r--r--   0        0        0     4962 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/storage_attributes.py
+-rw-r--r--   0        0        0    11779 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/support_zip_generator_request.py
+-rw-r--r--   0        0        0     4900 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/support_zip_xo.py
+-rw-r--r--   0        0        0     5353 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/tag_xo.py
+-rw-r--r--   0        0        0     7612 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/task_xo.py
+-rw-r--r--   0        0        0     6108 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/throwable.py
+-rw-r--r--   0        0        0    36352 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/update_ldap_server_xo.py
+-rw-r--r--   0        0        0     5819 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/upload_definition_xo.py
+-rw-r--r--   0        0        0     5934 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/upload_field_definition_xo.py
+-rw-r--r--   0        0        0     4299 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/user_tokens_api_model.py
+-rw-r--r--   0        0        0    40587 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/v1_components_body.py
+-rw-r--r--   0        0        0     4795 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_attributes.py
+-rw-r--r--   0        0        0     6964 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_group_repository_api_request.py
+-rw-r--r--   0        0        0     7385 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_hosted_api_repository.py
+-rw-r--r--   0        0        0     7694 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_hosted_repository_api_request.py
+-rw-r--r--   0        0        0    11415 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     4378 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_signing_repositories_attributes.py
+-rw-r--r--   0        0        0    13274 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/nxrm_sdk/rest.py
+-rw-r--r--   0        0        0      645 2023-06-03 15:00:29.782600 sonatype_nxrm_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3882 1970-01-01 00:00:00.000000 sonatype_nxrm_sdk-0.1.5/PKG-INFO
```

### Comparing `sonatype_nxrm_sdk-0.1.4/LICENSE` & `sonatype_nxrm_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/README.md` & `sonatype_nxrm_sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/__init__.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/__init__.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/assets_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/assets_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/azure_blob_store_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/azure_blob_store_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/blob_store_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/blob_store_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/components_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/components_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/content_selectors_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/content_selectors_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/email_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/email_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/formats_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/formats_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/lifecycle_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/lifecycle_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/manage_iq_server_configuration_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/manage_iq_server_configuration_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/product_licensing_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/product_licensing_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/read_only_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/read_only_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/replication_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/replication_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/repository_management_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/repository_management_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/routing_rules_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/routing_rules_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/script_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/script_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/search_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/search_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_atlassian_crowd_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_atlassian_crowd_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_certificates_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_certificates_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_anonymous_access_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_anonymous_access_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_jwt_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_jwt_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_ldap_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_ldap_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_privileges_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_privileges_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_realms_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_realms_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_roles_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_roles_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_saml_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_saml_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_user_tokens_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_user_tokens_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/security_management_users_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/security_management_users_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/staging_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/staging_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/status_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/status_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/support_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/support_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/tags_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api/tasks_api.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/api_client.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/configuration.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/__init__.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/abstract_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/abstract_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/anonymous_access_settings_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/anonymous_access_settings_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_certificate.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_certificate.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_create_user.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_create_user.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_email_configuration.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_email_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_email_validation.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_email_validation.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_license_details_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_license_details_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_application_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_application_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_admin_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_admin_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_content_selector_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_content_selector_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_repository_view_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_repository_view_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_script_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_script_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_privilege_wildcard_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_privilege_wildcard_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_user.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_user.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/api_user_source.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/api_user_source.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_repositories_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_repositories_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/apt_signing_repositories_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/apt_signing_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/asset_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/asset_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_authentication.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_authentication.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_bucket_configuration.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_blob_store_api_model.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/azure_connection_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/azure_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/base_tag_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/base_tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/blob_store_api_soft_quota.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/blob_store_api_soft_quota.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/blob_store_quota_result_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/blob_store_quota_result_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/bower_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/bower_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/cleanup_policy_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/cleanup_policy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/cocoapods_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/cocoapods_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/component_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/component_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/component_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/component_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/conan_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/conan_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/conda_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/conda_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_create_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_response.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/content_selector_api_update_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/content_selector_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/create_ldap_server_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/create_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/crowd_api_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/crowd_api_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_group_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_group_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_hosted_storage_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_hosted_storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/docker_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/docker_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_create_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_model.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/file_blob_store_api_update_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/file_blob_store_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/generic_blob_store_api_response.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/generic_blob_store_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/git_lfs_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/git_lfs_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/golang_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/golang_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/golang_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/golang_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_create_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_model.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_response.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_blob_store_api_update_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_blob_store_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/group_deploy_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/group_deploy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/helm_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/helm_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/helm_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/helm_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/hosted_storage_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/hosted_storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_attributes_with_preemptive_auth.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_attributes_with_preemptive_auth.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_authentication_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_authentication_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/http_client_connection_authentication_attributes_with_preemptive.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/http_client_connection_authentication_attributes_with_preemptive.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/input_stream.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/input_stream.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/iq_connection_verification_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/iq_connection_verification_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/iq_connection_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/iq_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_hosted_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/maven_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/maven_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/negative_cache_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/negative_cache_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/npm_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/npm_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_proxy_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/nuget_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/nuget_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/p2_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/p2_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_asset_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_asset_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_component_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_component_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_tag_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/page_task_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/page_task_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/proxy_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/proxy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/pypi_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/pypi_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/r_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/r_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/raw_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/raw_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/read_ldap_server_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/read_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/read_only_state.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/read_only_state.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/realm_api_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/realm_api_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_connection_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/replication_enable_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/replication_enable_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/repository_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/repository_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/result.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/result.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/role_xo_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/role_xo_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/role_xo_response.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/role_xo_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/routing_rule_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/routing_rule_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/ruby_gems_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/ruby_gems_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_advanced_bucket_connection.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_advanced_bucket_connection.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket_configuration.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_bucket_security.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_bucket_security.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_encryption.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_encryption.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/s3_blob_store_api_model.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/s3_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/saml_configuration_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/saml_configuration_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/script_result_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/script_result_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/script_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/script_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_group_deploy_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_group_deploy_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_group_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_group_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_hosted_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_hosted_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/simple_api_proxy_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/simple_api_proxy_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/stack_trace_element.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/storage_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/support_zip_generator_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/support_zip_generator_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/support_zip_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/support_zip_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/tag_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/task_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/task_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/throwable.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/throwable.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/update_ldap_server_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/update_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/upload_definition_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/upload_definition_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/upload_field_definition_xo.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/upload_field_definition_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/user_tokens_api_model.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/user_tokens_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/v1_components_body.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/v1_components_body.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_group_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_hosted_api_repository.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_hosted_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_proxy_repository_api_request.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/models/yum_signing_repositories_attributes.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/models/yum_signing_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/nxrm_sdk/rest.py` & `sonatype_nxrm_sdk-0.1.5/nxrm_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `sonatype_nxrm_sdk-0.1.4/pyproject.toml` & `sonatype_nxrm_sdk-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "sonatype-nxrm-sdk"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python SDK for Sonatype Nexus Repository Manager"
 authors = ["Justin Bailey <justthered63@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nxrm_sdk" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 certifi = "^2023.5.7"
 frozendict = "^2.3.8"
 python-dateutil = "^2.8.2"
 setuptools = "^67.8.0"
 typing-extensions = "^4.6.3"
+six = "^1.16.0"
 urllib3 = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
```

### Comparing `sonatype_nxrm_sdk-0.1.4/PKG-INFO` & `sonatype_nxrm_sdk-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sonatype-nxrm-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for Sonatype Nexus Repository Manager
 License: MIT
 Author: Justin Bailey
 Author-email: justthered63@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: urllib3 (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Sonatype: Nexus Repository Manager Python SDK
 
 - [Sonatype: Nexus Repository Manager Python SDK](#sonatype-nexus-repository-manager-python-sdk)
```

