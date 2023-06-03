# Comparing `tmp/fastapi-0.95.2.tar.gz` & `tmp/fastapi-0.96.0.tar.gz`

## Comparing `fastapi-0.95.2.tar` & `fastapi-0.96.0.tar`

### file list

```diff
@@ -1,1859 +1,1869 @@
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastapi-0.95.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.95.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.95.2/SECURITY.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/dependabot.yml
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/DISCUSSION_TEMPLATE/questions.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/ISSUE_TEMPLATE/privileged.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/notify-translations/Dockerfile
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/notify-translations/action.yml
--rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/notify-translations/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/people/Dockerfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/people/action.yml
--rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/people/app/main.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/watch-previews/Dockerfile
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/watch-previews/action.yml
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/actions/watch-previews/app/main.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/label-approved.yml
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/notify-translations.yml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/people.yml
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.95.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/missing-translation.md
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/az/mkdocs.yml
--rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/az/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/az/overrides/.gitignore
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/cs/mkdocs.yml
--rw-r--r--   0        0        0    19467 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/cs/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/cs/overrides/.gitignore
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/de/mkdocs.yml
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/de/docs/features.md
--rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/de/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/de/overrides/.gitignore
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/mkdocs.yml
--rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/alternatives.md
--rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/async.md
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/benchmarks.md
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/contributing.md
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/external-links.md
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/fastapi-people.md
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/features.md
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/help-fastapi.md
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/history-design-future.md
--rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/index.md
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/project-generation.md
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/python-types.md
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/events.md
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/graphql.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/index.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/middleware.md
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/settings.md
--rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/templates.md
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/security/index.md
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/concepts.md
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/deta.md
--rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/docker.md
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/https.md
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/index.md
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/manually.md
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/deployment/versions.md
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/body.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/index.md
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/em/overrides/.gitignore
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/mkdocs.yml
--rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/data/external_links.yml
--rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/data/github_sponsors.yml
--rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/data/people.yml
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/data/sponsors.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/data/sponsors_badge.yml
--rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/alternatives.md
--rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/async.md
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/benchmarks.md
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/contributing.md
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/external-links.md
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/fastapi-people.md
--rw-r--r--   0        0        0     9663 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/features.md
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/help-fastapi.md
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/history-design-future.md
--rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/index.md
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/newsletter.md
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/project-generation.md
--rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/python-types.md
--rw-r--r--   0        0        0   261378 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/release-notes.md
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/events.md
--rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/graphql.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/index.md
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/middleware.md
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/settings.md
--rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/templates.md
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/security/index.md
--rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/css/custom.css
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/css/termynal.css
--rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/concepts.md
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/deta.md
--rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/docker.md
--rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/https.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/index.md
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/manually.md
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/deployment/versions.md
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/icon-transparent-bg.png
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/icon-white-bg.png
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/icon-white.svg
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-teal-vector.svg
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-teal.svg
--rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/vscode-completion.png
--rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
--rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
--rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
--rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
--rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
--rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
--rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
--rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
--rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
--rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
--rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
--rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
--rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/concepts/image01.png
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/concepts/process-ram.drawio
--rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/concepts/process-ram.svg
--rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image01.png
--rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image02.png
--rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image03.png
--rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image04.png
--rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image05.png
--rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/deta/image06.png
--rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https.drawio
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https.svg
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https01.drawio
--rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https01.svg
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https02.drawio
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https02.svg
--rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https03.drawio
--rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https03.svg
--rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https04.drawio
--rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https04.svg
--rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https05.drawio
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https05.svg
--rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https06.drawio
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https06.svg
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https07.drawio
--rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https07.svg
--rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https08.drawio
--rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/deployment/https/https08.svg
--rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-01-swagger-ui-simple.png
--rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-02-redoc-simple.png
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-03-swagger-02.png
--rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-04-swagger-03.png
--rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-05-swagger-04.png
--rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/index/index-06-redoc-02.png
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal-vector.svg
--rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal.svg
--rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-white-bg.png
--rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image01.png
--rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image02.png
--rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image03.png
--rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image04.png
--rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image05.png
--rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/python-types/image06.png
--rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/budget-insight.svg
--rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/calmcode.jpg
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/classiq-banner.png
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/classiq.png
--rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/cryptapi-banner.svg
--rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/cryptapi.svg
--rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/databento.svg
--rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/deta-banner.svg
--rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/deta.svg
--rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/docarray-top-banner.svg
--rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/docarray.svg
--rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/doist-banner.svg
--rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/doist.svg
--rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/dropbase-banner.svg
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/dropbase.svg
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/exoflare.png
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
--rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/haystack-fastapi.svg
--rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/imgwhale-banner.svg
--rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/imgwhale.svg
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/ines-course.jpg
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/investsuite.svg
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina-ai-banner.png
--rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina-ai.png
--rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina-banner.svg
--rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina-top-banner.svg
--rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina.svg
--rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/jina2.svg
--rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/powens.png
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks-banner.png
--rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks.png
--rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks2.png
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/svix.svg
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/talkpython.png
--rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/testdriven.svg
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/vimso.png
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/sponsors/wetransfer.svg
--rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/additional-responses/image01.png
--rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/async-sql-databases/image01.png
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
--rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
--rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
--rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/image01.png
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/package.drawio
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/package.svg
--rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body/image01.png
--rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body/image02.png
--rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body/image03.png
--rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body/image04.png
--rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body/image05.png
--rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body-fields/image01.png
--rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body-fields/image02.png
--rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/body-nested-models/image01.png
--rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/custom-response/image01.png
--rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/dataclasses/image01.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/debugging/image01.png
--rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/debugging/image02.png
--rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/dependencies/image01.png
--rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/dependencies/image02.png
--rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image01.png
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image02.png
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image03.png
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image04.png
--rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image01.png
--rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image02.png
--rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image03.png
--rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image04.png
--rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image05.png
--rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image06.png
--rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image07.png
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image08.png
--rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/graphql/image01.png
--rw-r--r--   0        0        0    90062 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/metadata/image01.png
--rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/metadata/image02.png
--rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
--rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
--rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
--rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
--rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
--rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
--rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
--rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image01.png
--rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image02.png
--rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image03.png
--rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
--rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
--rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/response-model/image01.png
--rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/response-model/image02.png
--rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/response-status-code/image01.png
--rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/response-status-code/image02.png
--rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image01.png
--rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image02.png
--rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image03.png
--rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image04.png
--rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image05.png
--rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image06.png
--rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image07.png
--rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image08.png
--rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image09.png
--rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image10.png
--rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image11.png
--rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/security/image12.png
--rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/sql-databases/image01.png
--rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/sql-databases/image02.png
--rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/sub-applications/image01.png
--rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/sub-applications/image02.png
--rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image01.png
--rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image02.png
--rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image03.png
--rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image04.png
--rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image05.png
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/js/chat.js
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/js/termynal.js
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/body.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/index.md
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/query-params.md
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/testing.md
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/security/index.md
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/en/overrides/main.html
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/mkdocs.yml
--rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/async.md
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/features.md
--rw-r--r--   0        0        0    19594 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/index.md
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/python-types.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/advanced/index.md
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/advanced/response-directly.md
--rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/tutorial/index.md
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/docs/tutorial/query-params.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/es/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fa/mkdocs.yml
--rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fa/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fa/overrides/.gitignore
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/mkdocs.yml
--rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/alternatives.md
--rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/async.md
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/external-links.md
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/features.md
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/help-fastapi.md
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/history-design-future.md
--rw-r--r--   0        0        0    22777 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/index.md
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/project-generation.md
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/python-types.md
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/advanced/index.md
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/deta.md
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/docker.md
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/https.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/index.md
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/manually.md
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/deployment/versions.md
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/body.md
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/docs/tutorial/query-params.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/fr/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/he/mkdocs.yml
--rw-r--r--   0        0        0    21849 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/he/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/he/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/hy/mkdocs.yml
--rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/hy/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/hy/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/id/mkdocs.yml
--rw-r--r--   0        0        0    18622 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/id/docs/index.md
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/id/docs/tutorial/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/id/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/it/mkdocs.yml
--rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/it/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/it/overrides/.gitignore
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/mkdocs.yml
--rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/alternatives.md
--rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/async.md
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/benchmarks.md
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/contributing.md
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/external-links.md
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/fastapi-people.md
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/features.md
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/help-fastapi.md
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/history-design-future.md
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/index.md
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/project-generation.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/index.md
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/advanced/websockets.md
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/deployment/deta.md
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/deployment/docker.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/deployment/index.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/deployment/manually.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/deployment/versions.md
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/body.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/cors.md
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/index.md
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/middleware.md
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/testing.md
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ja/overrides/.gitignore
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/mkdocs.yml
--rw-r--r--   0        0        0    20074 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/index.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/deployment/versions.md
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/cors.md
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/encoder.md
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/index.md
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ko/overrides/.gitignore
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/lo/mkdocs.yml
--rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/lo/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/lo/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/nl/mkdocs.yml
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/nl/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/nl/overrides/.gitignore
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pl/mkdocs.yml
--rw-r--r--   0        0        0    20000 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pl/docs/index.md
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pl/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pl/docs/tutorial/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pl/overrides/.gitignore
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/mkdocs.yml
--rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/alternatives.md
--rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/async.md
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/benchmarks.md
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/contributing.md
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment.md
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/external-links.md
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/fastapi-people.md
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/features.md
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/help-fastapi.md
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/history-design-future.md
--rw-r--r--   0        0        0    19250 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/index.md
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/project-generation.md
--rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/python-types.md
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/advanced/events.md
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/advanced/index.md
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment/deta.md
--rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment/docker.md
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment/https.md
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment/index.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/deployment/versions.md
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/body.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/index.md
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/docs/tutorial/security/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/pt/overrides/.gitignore
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/mkdocs.yml
--rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/alternatives.md
--rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/async.md
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/benchmarks.md
--rw-r--r--   0        0        0    23067 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/contributing.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/external-links.md
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/fastapi-people.md
--rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/features.md
--rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/help-fastapi.md
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/history-design-future.md
--rw-r--r--   0        0        0    26659 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/index.md
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/project-generation.md
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/python-types.md
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/deployment/https.md
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/deployment/index.md
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/deployment/manually.md
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/deployment/versions.md
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/docs/tutorial/testing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ru/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sq/mkdocs.yml
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sq/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sq/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sv/mkdocs.yml
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sv/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/sv/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ta/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/ta/overrides/.gitignore
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/mkdocs.yml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/benchmarks.md
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/features.md
--rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/index.md
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/python-types.md
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/docs/tutorial/first_steps.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/tr/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/uk/mkdocs.yml
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/uk/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/uk/overrides/.gitignore
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/mkdocs.yml
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/benchmarks.md
--rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/contributing.md
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/fastapi-people.md
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/features.md
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/help-fastapi.md
--rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/index.md
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/python-types.md
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/custom-response.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/index.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/advanced/wsgi.md
--rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/body.md
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/index.md
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs/zh/overrides/.gitignore
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extending_openapi/tutorial002.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extending_openapi/tutorial003.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extending_openapi/tutorial004.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extending_openapi/tutorial005.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.95.2/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/__init__.py
--rw-r--r--   0        0        0    39525 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/applications.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/background.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/concurrency.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/datastructures.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/encoders.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/exception_handlers.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/exceptions.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/logger.py
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/param_functions.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/py.typed
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/requests.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/responses.py
--rw-r--r--   0        0        0    55563 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/routing.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/staticfiles.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/templating.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/testclient.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/types.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/dependencies/models.py
--rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/dependencies/utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/openapi/constants.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/openapi/docs.py
--rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/openapi/models.py
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/openapi/utils.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/__init__.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/api_key.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/base.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/http.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/oauth2.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.95.2/fastapi/security/utils.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/clean.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/docs-live.sh
--rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/docs.py
--rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/format.sh
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/gitter_releases_bot.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/lint.sh
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/notify.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/publish.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/test.sh
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi-0.95.2/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/__init__.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/main.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_properties.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_annotated.py
--rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_application.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_datastructures.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_empty_router.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_extra_routes.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_filter_pydantic_sub_model.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_get_request_body.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_include_route.py
--rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_local_docs.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_param_class.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_params_repr.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_path.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_put_no_body.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_query.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_required_noneable.py
--rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_route_scope.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_router_events.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0    33384 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_serialize_response.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tuples.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_union_body.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_validate_response.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_validate_response_recursive.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_ws_router.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.95.2/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.95.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.95.2/LICENSE
--rw-r--r--   0        0        0    20665 2020-02-02 00:00:00.000000 fastapi-0.95.2/README.md
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 fastapi-0.95.2/pyproject.toml
--rw-r--r--   0        0        0    24865 2020-02-02 00:00:00.000000 fastapi-0.95.2/PKG-INFO
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastapi-0.96.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.96.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.96.0/SECURITY.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/notify-translations/Dockerfile
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/notify-translations/action.yml
+-rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/notify-translations/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/people/Dockerfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/people/action.yml
+-rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/people/app/main.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/watch-previews/Dockerfile
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/watch-previews/action.yml
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/actions/watch-previews/app/main.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/label-approved.yml
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/notify-translations.yml
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/people.yml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.96.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/missing-translation.md
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/az/mkdocs.yml
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/az/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/az/overrides/.gitignore
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/cs/mkdocs.yml
+-rw-r--r--   0        0        0    19467 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/cs/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/cs/overrides/.gitignore
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/de/mkdocs.yml
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/de/docs/features.md
+-rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/de/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/de/overrides/.gitignore
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/mkdocs.yml
+-rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/alternatives.md
+-rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/async.md
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/benchmarks.md
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/contributing.md
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/external-links.md
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/fastapi-people.md
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/features.md
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/help-fastapi.md
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/history-design-future.md
+-rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/index.md
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/project-generation.md
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/python-types.md
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/events.md
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/graphql.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/index.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/settings.md
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/templates.md
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/concepts.md
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/deta.md
+-rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/docker.md
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/https.md
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/index.md
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/manually.md
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/deployment/versions.md
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/index.md
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/em/overrides/.gitignore
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/data/external_links.yml
+-rw-r--r--   0        0        0    25966 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/data/github_sponsors.yml
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/data/people.yml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/data/sponsors.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/data/sponsors_badge.yml
+-rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/alternatives.md
+-rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/async.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/benchmarks.md
+-rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/contributing.md
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/external-links.md
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9663 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/features.md
+-rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/history-design-future.md
+-rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/index.md
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/newsletter.md
+-rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/project-generation.md
+-rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/python-types.md
+-rw-r--r--   0        0        0   264355 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/release-notes.md
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/events.md
+-rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/graphql.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/index.md
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/settings.md
+-rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/templates.md
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/css/custom.css
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/css/termynal.css
+-rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/deta.md
+-rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/docker.md
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/https.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/index.md
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/manually.md
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/deployment/versions.md
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/icon-transparent-bg.png
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/icon-white-bg.png
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-teal-vector.svg
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-teal.svg
+-rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
+-rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
+-rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
+-rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
+-rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
+-rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
+-rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
+-rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
+-rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
+-rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
+-rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
+-rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
+-rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/concepts/image01.png
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/concepts/process-ram.drawio
+-rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/concepts/process-ram.svg
+-rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image01.png
+-rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image02.png
+-rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image03.png
+-rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image04.png
+-rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image05.png
+-rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/deta/image06.png
+-rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https.drawio
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https.svg
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https01.drawio
+-rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https01.svg
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https02.drawio
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https02.svg
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https03.drawio
+-rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https03.svg
+-rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https04.drawio
+-rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https04.svg
+-rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https05.drawio
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https05.svg
+-rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https06.drawio
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https06.svg
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https07.drawio
+-rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https07.svg
+-rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https08.drawio
+-rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/deployment/https/https08.svg
+-rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png
+-rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-02-redoc-simple.png
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-03-swagger-02.png
+-rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-04-swagger-03.png
+-rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-05-swagger-04.png
+-rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/index/index-06-redoc-02.png
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal.svg
+-rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-white-bg.png
+-rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image01.png
+-rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image02.png
+-rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image03.png
+-rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image04.png
+-rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image05.png
+-rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/python-types/image06.png
+-rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/budget-insight.svg
+-rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/calmcode.jpg
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/classiq-banner.png
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/classiq.png
+-rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/cryptapi-banner.svg
+-rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/cryptapi.svg
+-rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/databento.svg
+-rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/deta-banner.svg
+-rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/deta.svg
+-rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/docarray-top-banner.svg
+-rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/docarray.svg
+-rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/doist-banner.svg
+-rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/doist.svg
+-rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/dropbase-banner.svg
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/dropbase.svg
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/exoflare.png
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
+-rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/haystack-fastapi.svg
+-rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/imgwhale-banner.svg
+-rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/imgwhale.svg
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/ines-course.jpg
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/investsuite.svg
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina-ai-banner.png
+-rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina-ai.png
+-rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina-banner.svg
+-rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina-top-banner.svg
+-rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina.svg
+-rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/jina2.svg
+-rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/powens.png
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks-banner.png
+-rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks.png
+-rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks2.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/svix.svg
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/talkpython.png
+-rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/testdriven.svg
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/vimso.png
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/sponsors/wetransfer.svg
+-rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/additional-responses/image01.png
+-rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
+-rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
+-rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
+-rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/image01.png
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/package.svg
+-rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body/image01.png
+-rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body/image02.png
+-rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body/image03.png
+-rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body/image04.png
+-rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body/image05.png
+-rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body-fields/image01.png
+-rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body-fields/image02.png
+-rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/body-nested-models/image01.png
+-rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/custom-response/image01.png
+-rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/dataclasses/image01.png
+-rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/debugging/image01.png
+-rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/debugging/image02.png
+-rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/dependencies/image01.png
+-rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/dependencies/image02.png
+-rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image01.png
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image02.png
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image03.png
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image04.png
+-rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image01.png
+-rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image02.png
+-rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image03.png
+-rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image04.png
+-rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image05.png
+-rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image06.png
+-rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image07.png
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image08.png
+-rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/graphql/image01.png
+-rw-r--r--   0        0        0    90062 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/metadata/image01.png
+-rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/metadata/image02.png
+-rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
+-rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
+-rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
+-rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
+-rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
+-rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
+-rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
+-rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image01.png
+-rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image02.png
+-rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image03.png
+-rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
+-rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
+-rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/response-model/image01.png
+-rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/response-model/image02.png
+-rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/response-status-code/image01.png
+-rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/response-status-code/image02.png
+-rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image01.png
+-rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image02.png
+-rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image03.png
+-rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image04.png
+-rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image05.png
+-rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image06.png
+-rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image07.png
+-rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image08.png
+-rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image09.png
+-rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image10.png
+-rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image11.png
+-rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/security/image12.png
+-rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/sql-databases/image01.png
+-rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/sql-databases/image02.png
+-rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/sub-applications/image01.png
+-rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/sub-applications/image02.png
+-rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image01.png
+-rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image02.png
+-rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image03.png
+-rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image04.png
+-rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image05.png
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/js/chat.js
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/js/termynal.js
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/en/overrides/main.html
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/mkdocs.yml
+-rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/async.md
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/features.md
+-rw-r--r--   0        0        0    19594 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/index.md
+-rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/python-types.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/advanced/index.md
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/tutorial/index.md
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/es/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fa/mkdocs.yml
+-rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fa/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fa/overrides/.gitignore
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/mkdocs.yml
+-rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/alternatives.md
+-rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/async.md
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/external-links.md
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/features.md
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/history-design-future.md
+-rw-r--r--   0        0        0    22777 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/index.md
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/project-generation.md
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/python-types.md
+-rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/advanced/index.md
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/deta.md
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/docker.md
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/https.md
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/index.md
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/fr/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/he/mkdocs.yml
+-rw-r--r--   0        0        0    21849 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/he/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/he/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/hy/mkdocs.yml
+-rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/hy/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/hy/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/id/mkdocs.yml
+-rw-r--r--   0        0        0    18622 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/id/docs/index.md
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/id/docs/tutorial/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/id/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/it/mkdocs.yml
+-rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/it/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/it/overrides/.gitignore
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/mkdocs.yml
+-rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/alternatives.md
+-rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/async.md
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/benchmarks.md
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/contributing.md
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/external-links.md
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/fastapi-people.md
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/features.md
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/history-design-future.md
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/index.md
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/project-generation.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/index.md
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/deployment/deta.md
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/deployment/docker.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/deployment/index.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ja/overrides/.gitignore
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/mkdocs.yml
+-rw-r--r--   0        0        0    20074 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/index.md
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ko/overrides/.gitignore
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/lo/mkdocs.yml
+-rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/lo/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/lo/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/nl/mkdocs.yml
+-rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/nl/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/nl/overrides/.gitignore
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pl/mkdocs.yml
+-rw-r--r--   0        0        0    20000 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pl/docs/index.md
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pl/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pl/docs/tutorial/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pl/overrides/.gitignore
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/mkdocs.yml
+-rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/alternatives.md
+-rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/async.md
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/benchmarks.md
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/contributing.md
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment.md
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/external-links.md
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/fastapi-people.md
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/features.md
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/history-design-future.md
+-rw-r--r--   0        0        0    19250 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/index.md
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/project-generation.md
+-rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/python-types.md
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/advanced/events.md
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/advanced/index.md
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment/deta.md
+-rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment/docker.md
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment/https.md
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment/index.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/index.md
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/pt/overrides/.gitignore
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/mkdocs.yml
+-rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/alternatives.md
+-rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/async.md
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/benchmarks.md
+-rw-r--r--   0        0        0    23067 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/contributing.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/external-links.md
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/fastapi-people.md
+-rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/features.md
+-rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/help-fastapi.md
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/history-design-future.md
+-rw-r--r--   0        0        0    26659 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/index.md
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/project-generation.md
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/python-types.md
+-rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/deployment/https.md
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/deployment/index.md
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/deployment/manually.md
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/deployment/versions.md
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/docs/tutorial/testing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ru/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sq/mkdocs.yml
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sq/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sq/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sv/mkdocs.yml
+-rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sv/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/sv/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ta/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/ta/overrides/.gitignore
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/mkdocs.yml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/benchmarks.md
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/features.md
+-rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/index.md
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/python-types.md
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/docs/tutorial/first_steps.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/tr/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/uk/mkdocs.yml
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/uk/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/uk/overrides/.gitignore
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/mkdocs.yml
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/benchmarks.md
+-rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/contributing.md
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/features.md
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/help-fastapi.md
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/index.md
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/python-types.md
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/index.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs/zh/overrides/.gitignore
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extending_openapi/tutorial002.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extending_openapi/tutorial003.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extending_openapi/tutorial004.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extending_openapi/tutorial005.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.96.0/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/__init__.py
+-rw-r--r--   0        0        0    39525 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/applications.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/background.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/concurrency.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/datastructures.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/encoders.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/exception_handlers.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/exceptions.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/logger.py
+-rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/param_functions.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/py.typed
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/requests.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/responses.py
+-rw-r--r--   0        0        0    55563 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/routing.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/templating.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/testclient.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/types.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/dependencies/models.py
+-rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/dependencies/utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/openapi/constants.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/openapi/docs.py
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/openapi/models.py
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/openapi/utils.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/__init__.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/api_key.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/base.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/http.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/oauth2.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.96.0/fastapi/security/utils.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/clean.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/docs-live.sh
+-rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/docs.py
+-rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/format.sh
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/gitter_releases_bot.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/notify.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/test.sh
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi-0.96.0/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/__init__.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/main.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_annotated.py
+-rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_application.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_datastructures.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_extra_routes.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_filter_pydantic_sub_model.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_include_route.py
+-rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_local_docs.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_param_class.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_params_repr.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_path.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_put_no_body.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_query.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_router_events.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0    33384 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tuples.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_union_body.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_validate_response_recursive.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_ws_router.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.96.0/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.96.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.96.0/LICENSE
+-rw-r--r--   0        0        0    20495 2020-02-02 00:00:00.000000 fastapi-0.96.0/README.md
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 fastapi-0.96.0/pyproject.toml
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 fastapi-0.96.0/PKG-INFO
```

### Comparing `fastapi-0.95.2/.pre-commit-config.yaml` & `fastapi-0.96.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/SECURITY.md` & `fastapi-0.96.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/DISCUSSION_TEMPLATE/questions.yml` & `fastapi-0.96.0/.github/DISCUSSION_TEMPLATE/questions.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/ISSUE_TEMPLATE/config.yml` & `fastapi-0.96.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/ISSUE_TEMPLATE/privileged.yml` & `fastapi-0.96.0/.github/ISSUE_TEMPLATE/privileged.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/actions/comment-docs-preview-in-pr/app/main.py` & `fastapi-0.96.0/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/actions/notify-translations/app/main.py` & `fastapi-0.96.0/.github/actions/notify-translations/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/actions/people/app/main.py` & `fastapi-0.96.0/.github/actions/people/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/actions/watch-previews/app/main.py` & `fastapi-0.96.0/.github/actions/watch-previews/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/build-docs.yml` & `fastapi-0.96.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/issue-manager.yml` & `fastapi-0.96.0/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/latest-changes.yml` & `fastapi-0.96.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/notify-translations.yml` & `fastapi-0.96.0/.github/workflows/notify-translations.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/people.yml` & `fastapi-0.96.0/.github/workflows/people.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/preview-docs.yml` & `fastapi-0.96.0/.github/workflows/preview-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/publish.yml` & `fastapi-0.96.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/smokeshow.yml` & `fastapi-0.96.0/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/.github/workflows/test.yml` & `fastapi-0.96.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/az/mkdocs.yml` & `fastapi-0.96.0/docs/az/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/az/docs/index.md` & `fastapi-0.96.0/docs/az/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/cs/mkdocs.yml` & `fastapi-0.96.0/docs/cs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/cs/docs/index.md` & `fastapi-0.96.0/docs/cs/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/de/mkdocs.yml` & `fastapi-0.96.0/docs/de/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/de/docs/features.md` & `fastapi-0.96.0/docs/de/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/de/docs/index.md` & `fastapi-0.96.0/docs/de/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/mkdocs.yml` & `fastapi-0.96.0/docs/em/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/alternatives.md` & `fastapi-0.96.0/docs/em/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/async.md` & `fastapi-0.96.0/docs/em/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/benchmarks.md` & `fastapi-0.96.0/docs/em/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/contributing.md` & `fastapi-0.96.0/docs/em/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/external-links.md` & `fastapi-0.96.0/docs/em/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/fastapi-people.md` & `fastapi-0.96.0/docs/em/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/features.md` & `fastapi-0.96.0/docs/em/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/help-fastapi.md` & `fastapi-0.96.0/docs/em/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/history-design-future.md` & `fastapi-0.96.0/docs/em/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/index.md` & `fastapi-0.96.0/docs/em/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/project-generation.md` & `fastapi-0.96.0/docs/em/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/python-types.md` & `fastapi-0.96.0/docs/em/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/additional-responses.md` & `fastapi-0.96.0/docs/em/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/em/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/advanced-dependencies.md` & `fastapi-0.96.0/docs/em/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/async-sql-databases.md` & `fastapi-0.96.0/docs/em/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/async-tests.md` & `fastapi-0.96.0/docs/em/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/behind-a-proxy.md` & `fastapi-0.96.0/docs/em/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/conditional-openapi.md` & `fastapi-0.96.0/docs/em/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/custom-request-and-route.md` & `fastapi-0.96.0/docs/em/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/custom-response.md` & `fastapi-0.96.0/docs/em/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/dataclasses.md` & `fastapi-0.96.0/docs/em/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/events.md` & `fastapi-0.96.0/docs/em/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/extending-openapi.md` & `fastapi-0.96.0/docs/em/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/generate-clients.md` & `fastapi-0.96.0/docs/em/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/graphql.md` & `fastapi-0.96.0/docs/em/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/index.md` & `fastapi-0.96.0/docs/em/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/middleware.md` & `fastapi-0.96.0/docs/em/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/nosql-databases.md` & `fastapi-0.96.0/docs/em/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/openapi-callbacks.md` & `fastapi-0.96.0/docs/em/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/em/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/response-change-status-code.md` & `fastapi-0.96.0/docs/em/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/response-cookies.md` & `fastapi-0.96.0/docs/em/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/em/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/response-headers.md` & `fastapi-0.96.0/docs/em/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/settings.md` & `fastapi-0.96.0/docs/em/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/sql-databases-peewee.md` & `fastapi-0.96.0/docs/em/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/sub-applications.md` & `fastapi-0.96.0/docs/em/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/templates.md` & `fastapi-0.96.0/docs/em/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/testing-database.md` & `fastapi-0.96.0/docs/em/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/testing-dependencies.md` & `fastapi-0.96.0/docs/em/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/using-request-directly.md` & `fastapi-0.96.0/docs/em/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/websockets.md` & `fastapi-0.96.0/docs/em/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/wsgi.md` & `fastapi-0.96.0/docs/em/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/security/http-basic-auth.md` & `fastapi-0.96.0/docs/em/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.96.0/docs/em/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/concepts.md` & `fastapi-0.96.0/docs/em/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/deta.md` & `fastapi-0.96.0/docs/em/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/docker.md` & `fastapi-0.96.0/docs/em/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/https.md` & `fastapi-0.96.0/docs/em/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/index.md` & `fastapi-0.96.0/docs/em/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/manually.md` & `fastapi-0.96.0/docs/em/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/server-workers.md` & `fastapi-0.96.0/docs/em/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/deployment/versions.md` & `fastapi-0.96.0/docs/em/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/background-tasks.md` & `fastapi-0.96.0/docs/em/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/bigger-applications.md` & `fastapi-0.96.0/docs/em/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/body-fields.md` & `fastapi-0.96.0/docs/em/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/body-multiple-params.md` & `fastapi-0.96.0/docs/em/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/body-nested-models.md` & `fastapi-0.96.0/docs/em/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/body-updates.md` & `fastapi-0.96.0/docs/em/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/body.md` & `fastapi-0.96.0/docs/em/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/em/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/cors.md` & `fastapi-0.96.0/docs/em/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/debugging.md` & `fastapi-0.96.0/docs/em/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/encoder.md` & `fastapi-0.96.0/docs/em/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/extra-data-types.md` & `fastapi-0.96.0/docs/em/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/extra-models.md` & `fastapi-0.96.0/docs/em/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/em/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/handling-errors.md` & `fastapi-0.96.0/docs/em/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/em/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/index.md` & `fastapi-0.96.0/docs/em/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/metadata.md` & `fastapi-0.96.0/docs/em/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/middleware.md` & `fastapi-0.96.0/docs/em/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/path-operation-configuration.md` & `fastapi-0.96.0/docs/em/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.96.0/docs/em/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/em/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/em/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/em/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/request-files.md` & `fastapi-0.96.0/docs/em/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/request-forms-and-files.md` & `fastapi-0.96.0/docs/em/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/request-forms.md` & `fastapi-0.96.0/docs/em/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/response-model.md` & `fastapi-0.96.0/docs/em/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/em/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/schema-extra-example.md` & `fastapi-0.96.0/docs/em/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/sql-databases.md` & `fastapi-0.96.0/docs/em/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/static-files.md` & `fastapi-0.96.0/docs/em/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/testing.md` & `fastapi-0.96.0/docs/em/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/index.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.96.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/security/first-steps.md` & `fastapi-0.96.0/docs/em/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/security/get-current-user.md` & `fastapi-0.96.0/docs/em/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/security/index.md` & `fastapi-0.96.0/docs/em/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.96.0/docs/em/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/em/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.96.0/docs/em/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/mkdocs.yml` & `fastapi-0.96.0/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/data/external_links.yml` & `fastapi-0.96.0/docs/en/data/external_links.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/data/github_sponsors.yml` & `fastapi-0.96.0/docs/en/data/github_sponsors.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,77 +1,62 @@
 sponsors:
-- - login: jina-ai
-    avatarUrl: https://avatars.githubusercontent.com/u/60539444?v=4
-    url: https://github.com/jina-ai
-- - login: armand-sauzay
-    avatarUrl: https://avatars.githubusercontent.com/u/35524799?u=56e3e944bfe62770d1709c09552d2efc6d285ca6&v=4
-    url: https://github.com/armand-sauzay
 - - login: cryptapi
     avatarUrl: https://avatars.githubusercontent.com/u/44925437?u=61369138589bc7fee6c417f3fbd50fbd38286cc4&v=4
     url: https://github.com/cryptapi
 - - login: nihpo
     avatarUrl: https://avatars.githubusercontent.com/u/1841030?u=0264956d7580f7e46687a762a7baa629f84cf97c&v=4
     url: https://github.com/nihpo
   - login: ObliviousAI
     avatarUrl: https://avatars.githubusercontent.com/u/65656077?v=4
     url: https://github.com/ObliviousAI
-  - login: chaserowbotham
-    avatarUrl: https://avatars.githubusercontent.com/u/97751084?v=4
-    url: https://github.com/chaserowbotham
 - - login: mikeckennedy
     avatarUrl: https://avatars.githubusercontent.com/u/2035561?u=1bb18268bcd4d9249e1f783a063c27df9a84c05b&v=4
     url: https://github.com/mikeckennedy
   - login: deta
     avatarUrl: https://avatars.githubusercontent.com/u/47275976?v=4
     url: https://github.com/deta
   - login: deepset-ai
     avatarUrl: https://avatars.githubusercontent.com/u/51827949?v=4
     url: https://github.com/deepset-ai
-  - login: investsuite
-    avatarUrl: https://avatars.githubusercontent.com/u/73833632?v=4
-    url: https://github.com/investsuite
   - login: svix
     avatarUrl: https://avatars.githubusercontent.com/u/80175132?v=4
     url: https://github.com/svix
+  - login: databento-bot
+    avatarUrl: https://avatars.githubusercontent.com/u/98378480?u=494f679996e39427f7ddb1a7de8441b7c96fb670&v=4
+    url: https://github.com/databento-bot
   - login: VincentParedes
     avatarUrl: https://avatars.githubusercontent.com/u/103889729?v=4
     url: https://github.com/VincentParedes
 - - login: getsentry
     avatarUrl: https://avatars.githubusercontent.com/u/1396951?v=4
     url: https://github.com/getsentry
-- - login: InesIvanova
-    avatarUrl: https://avatars.githubusercontent.com/u/22920417?u=409882ec1df6dbd77455788bb383a8de223dbf6f&v=4
-    url: https://github.com/InesIvanova
-- - login: vyos
-    avatarUrl: https://avatars.githubusercontent.com/u/5647000?v=4
-    url: https://github.com/vyos
-  - login: takashi-yoneya
+- - login: takashi-yoneya
     avatarUrl: https://avatars.githubusercontent.com/u/33813153?u=2d0522bceba0b8b69adf1f2db866503bd96f944e&v=4
     url: https://github.com/takashi-yoneya
+  - login: mercedes-benz
+    avatarUrl: https://avatars.githubusercontent.com/u/34240465?v=4
+    url: https://github.com/mercedes-benz
   - login: xoflare
     avatarUrl: https://avatars.githubusercontent.com/u/74335107?v=4
     url: https://github.com/xoflare
+  - login: marvin-robot
+    avatarUrl: https://avatars.githubusercontent.com/u/41086007?u=091c5cb75af363123d66f58194805a97220ee1a7&v=4
+    url: https://github.com/marvin-robot
   - login: BoostryJP
     avatarUrl: https://avatars.githubusercontent.com/u/57932412?v=4
     url: https://github.com/BoostryJP
-- - login: johnadjei
-    avatarUrl: https://avatars.githubusercontent.com/u/767860?v=4
-    url: https://github.com/johnadjei
-  - login: HiredScore
+- - login: HiredScore
     avatarUrl: https://avatars.githubusercontent.com/u/3908850?v=4
     url: https://github.com/HiredScore
-  - login: ianshan0915
-    avatarUrl: https://avatars.githubusercontent.com/u/5893101?u=a178d247d882578b1d1ef214b2494e52eb28634c&v=4
-    url: https://github.com/ianshan0915
   - login: Trivie
     avatarUrl: https://avatars.githubusercontent.com/u/8161763?v=4
     url: https://github.com/Trivie
-  - login: Lovage-Labs
-    avatarUrl: https://avatars.githubusercontent.com/u/71685552?v=4
-    url: https://github.com/Lovage-Labs
+- - login: JonasKs
+    avatarUrl: https://avatars.githubusercontent.com/u/5310116?u=98a049f3e1491bffb91e1feb7e93def6881a9389&v=4
+    url: https://github.com/JonasKs
 - - login: moellenbeck
     avatarUrl: https://avatars.githubusercontent.com/u/169372?v=4
     url: https://github.com/moellenbeck
   - login: birkjernstrom
     avatarUrl: https://avatars.githubusercontent.com/u/281715?u=4be14b43f76b4bd497b1941309bb390250b405e6&v=4
     url: https://github.com/birkjernstrom
   - login: AccentDesign
@@ -79,20 +64,17 @@
     url: https://github.com/AccentDesign
   - login: RodneyU215
     avatarUrl: https://avatars.githubusercontent.com/u/3329665?u=ec6a9adf8e7e8e306eed7d49687c398608d1604f&v=4
     url: https://github.com/RodneyU215
   - login: tizz98
     avatarUrl: https://avatars.githubusercontent.com/u/5739698?u=f095a3659e3a8e7c69ccd822696990b521ea25f9&v=4
     url: https://github.com/tizz98
-  - login: dorianturba
-    avatarUrl: https://avatars.githubusercontent.com/u/9381120?u=4bfc7032a824d1ed1994aa8256dfa597c8f187ad&v=4
-    url: https://github.com/dorianturba
-  - login: jmaralc
-    avatarUrl: https://avatars.githubusercontent.com/u/21101214?u=b15a9f07b7cbf6c9dcdbcb6550bbd2c52f55aa50&v=4
-    url: https://github.com/jmaralc
+  - login: americanair
+    avatarUrl: https://avatars.githubusercontent.com/u/12281813?v=4
+    url: https://github.com/americanair
   - login: mainframeindustries
     avatarUrl: https://avatars.githubusercontent.com/u/55092103?v=4
     url: https://github.com/mainframeindustries
 - - login: povilasb
     avatarUrl: https://avatars.githubusercontent.com/u/1213442?u=b11f58ed6ceea6e8297c9b310030478ebdac894d&v=4
     url: https://github.com/povilasb
   - login: primer-io
@@ -128,46 +110,37 @@
   - login: wshayes
     avatarUrl: https://avatars.githubusercontent.com/u/365303?u=07ca03c5ee811eb0920e633cc3c3db73dbec1aa5&v=4
     url: https://github.com/wshayes
   - login: koxudaxi
     avatarUrl: https://avatars.githubusercontent.com/u/630670?u=507d8577b4b3670546b449c4c2ccbc5af40d72f7&v=4
     url: https://github.com/koxudaxi
   - login: falkben
-    avatarUrl: https://avatars.githubusercontent.com/u/653031?u=0c8d8f33d87f1aa1a6488d3f02105e9abc838105&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/653031?u=ad9838e089058c9e5a0bab94c0eec7cc181e0cd0&v=4
     url: https://github.com/falkben
   - login: jqueguiner
     avatarUrl: https://avatars.githubusercontent.com/u/690878?u=bd65cc1f228ce6455e56dfaca3ef47c33bc7c3b0&v=4
     url: https://github.com/jqueguiner
   - login: iobruno
     avatarUrl: https://avatars.githubusercontent.com/u/901651?u=460bc34ac298dca9870aafe3a1560a2ae789bc4a&v=4
     url: https://github.com/iobruno
   - login: tcsmith
     avatarUrl: https://avatars.githubusercontent.com/u/989034?u=7d8d741552b3279e8f4d3878679823a705a46f8f&v=4
     url: https://github.com/tcsmith
   - login: mrkmcknz
     avatarUrl: https://avatars.githubusercontent.com/u/1089376?u=2b9b8a8c25c33a4f6c220095638bd821cdfd13a3&v=4
     url: https://github.com/mrkmcknz
-  - login: coffeewasmyidea
-    avatarUrl: https://avatars.githubusercontent.com/u/1636488?u=8e32a4f200eff54dd79cd79d55d254bfce5e946d&v=4
-    url: https://github.com/coffeewasmyidea
+  - login: mickaelandrieu
+    avatarUrl: https://avatars.githubusercontent.com/u/1247388?u=599f6e73e452a9453f2bd91e5c3100750e731ad4&v=4
+    url: https://github.com/mickaelandrieu
   - login: jonakoudijs
     avatarUrl: https://avatars.githubusercontent.com/u/1906344?u=5ca0c9a1a89b6a2ba31abe35c66bdc07af60a632&v=4
     url: https://github.com/jonakoudijs
-  - login: corleyma
-    avatarUrl: https://avatars.githubusercontent.com/u/2080732?u=c61f9a4bbc45a45f5d855f93e5f6e0fc8b32c468&v=4
-    url: https://github.com/corleyma
-  - login: andre1sk
-    avatarUrl: https://avatars.githubusercontent.com/u/3148093?v=4
-    url: https://github.com/andre1sk
   - login: Shark009
     avatarUrl: https://avatars.githubusercontent.com/u/3163309?u=0c6f4091b0eda05c44c390466199826e6dc6e431&v=4
     url: https://github.com/Shark009
-  - login: ColliotL
-    avatarUrl: https://avatars.githubusercontent.com/u/3412402?u=ca64b07ecbef2f9da1cc2cac3f37522aa4814902&v=4
-    url: https://github.com/ColliotL
   - login: dblackrun
     avatarUrl: https://avatars.githubusercontent.com/u/3528486?v=4
     url: https://github.com/dblackrun
   - login: zsinx6
     avatarUrl: https://avatars.githubusercontent.com/u/3532625?u=ba75a5dc744d1116ccfeaaf30d41cb2fe81fe8dd&v=4
     url: https://github.com/zsinx6
   - login: aacayaco
@@ -199,77 +172,56 @@
     url: https://github.com/Yaleesa
   - login: iwpnd
     avatarUrl: https://avatars.githubusercontent.com/u/6152183?u=c485eefca5c6329600cae63dd35e4f5682ce6924&v=4
     url: https://github.com/iwpnd
   - login: simw
     avatarUrl: https://avatars.githubusercontent.com/u/6322526?v=4
     url: https://github.com/simw
-  - login: pkucmus
-    avatarUrl: https://avatars.githubusercontent.com/u/6347418?u=98f5918b32e214a168a2f5d59b0b8ebdf57dca0d&v=4
-    url: https://github.com/pkucmus
-  - login: s3ich4n
-    avatarUrl: https://avatars.githubusercontent.com/u/6926298?u=6690c5403bc1d9a1837886defdc5256e9a43b1db&v=4
-    url: https://github.com/s3ich4n
   - login: Rehket
     avatarUrl: https://avatars.githubusercontent.com/u/7015688?u=3afb0ba200feebbc7f958950e92db34df2a3c172&v=4
     url: https://github.com/Rehket
-  - login: ValentinCalomme
-    avatarUrl: https://avatars.githubusercontent.com/u/7288672?u=e09758c7a36c49f0fb3574abe919cbd344fdc2d6&v=4
-    url: https://github.com/ValentinCalomme
   - login: hiancdtrsnm
     avatarUrl: https://avatars.githubusercontent.com/u/7343177?v=4
     url: https://github.com/hiancdtrsnm
   - login: Shackelford-Arden
     avatarUrl: https://avatars.githubusercontent.com/u/7362263?v=4
     url: https://github.com/Shackelford-Arden
+  - login: savannahostrowski
+    avatarUrl: https://avatars.githubusercontent.com/u/8949415?u=c3177aa099fb2b8c36aeba349278b77f9a8df211&v=4
+    url: https://github.com/savannahostrowski
   - login: wdwinslow
     avatarUrl: https://avatars.githubusercontent.com/u/11562137?u=dc01daafb354135603a263729e3d26d939c0c452&v=4
     url: https://github.com/wdwinslow
-  - login: svats2k
-    avatarUrl: https://avatars.githubusercontent.com/u/12378398?u=ecf28c19f61052e664bdfeb2391f8107d137915c&v=4
-    url: https://github.com/svats2k
   - login: dannywade
     avatarUrl: https://avatars.githubusercontent.com/u/13680237?u=418ee985bd41577b20fde81417fb2d901e875e8a&v=4
     url: https://github.com/dannywade
   - login: khadrawy
     avatarUrl: https://avatars.githubusercontent.com/u/13686061?u=59f25ef42ecf04c22657aac4238ce0e2d3d30304&v=4
     url: https://github.com/khadrawy
-  - login: pablonnaoji
-    avatarUrl: https://avatars.githubusercontent.com/u/15187159?u=7480e0eaf959e9c5dfe3a05286f2ea4588c0a3c6&v=4
-    url: https://github.com/pablonnaoji
   - login: mjohnsey
     avatarUrl: https://avatars.githubusercontent.com/u/16784016?u=38fad2e6b411244560b3af99c5f5a4751bc81865&v=4
     url: https://github.com/mjohnsey
-  - login: abdalla19977
-    avatarUrl: https://avatars.githubusercontent.com/u/17257234?v=4
-    url: https://github.com/abdalla19977
   - login: wedwardbeck
     avatarUrl: https://avatars.githubusercontent.com/u/19333237?u=1de4ae2bf8d59eb4c013f21d863cbe0f2010575f&v=4
     url: https://github.com/wedwardbeck
+  - login: RaamEEIL
+    avatarUrl: https://avatars.githubusercontent.com/u/20320552?v=4
+    url: https://github.com/RaamEEIL
   - login: Filimoa
     avatarUrl: https://avatars.githubusercontent.com/u/21352040?u=0be845711495bbd7b756e13fcaeb8efc1ebd78ba&v=4
     url: https://github.com/Filimoa
   - login: shuheng-liu
     avatarUrl: https://avatars.githubusercontent.com/u/22414322?u=813c45f30786c6b511b21a661def025d8f7b609e&v=4
     url: https://github.com/shuheng-liu
-  - login: Pablongo24
-    avatarUrl: https://avatars.githubusercontent.com/u/24843427?u=78a6798469889d7a0690449fc667c39e13d5c6a9&v=4
-    url: https://github.com/Pablongo24
-  - login: Joeriksson
-    avatarUrl: https://avatars.githubusercontent.com/u/25037079?v=4
-    url: https://github.com/Joeriksson
-  - login: cometa-haley
-    avatarUrl: https://avatars.githubusercontent.com/u/25950317?u=cec1a3e0643b785288ae8260cc295a85ab344995&v=4
-    url: https://github.com/cometa-haley
+  - login: SebTota
+    avatarUrl: https://avatars.githubusercontent.com/u/25122511?v=4
+    url: https://github.com/SebTota
   - login: LarryGF
     avatarUrl: https://avatars.githubusercontent.com/u/26148349?u=431bb34d36d41c172466252242175281ae132152&v=4
     url: https://github.com/LarryGF
-  - login: veprimk
-    avatarUrl: https://avatars.githubusercontent.com/u/29689749?u=f8cb5a15a286e522e5b189bc572d5a1a90217fb2&v=4
-    url: https://github.com/veprimk
   - login: BrettskiPy
     avatarUrl: https://avatars.githubusercontent.com/u/30988215?u=d8a94a67e140d5ee5427724b292cc52d8827087a&v=4
     url: https://github.com/BrettskiPy
   - login: mauroalejandrojm
     avatarUrl: https://avatars.githubusercontent.com/u/31569442?u=cdada990a1527926a36e95f62c30a8b48bbc49a1&v=4
     url: https://github.com/mauroalejandrojm
   - login: Leay15
@@ -286,47 +238,38 @@
     url: https://github.com/ProteinQure
   - login: askurihin
     avatarUrl: https://avatars.githubusercontent.com/u/37978981?v=4
     url: https://github.com/askurihin
   - login: arleybri18
     avatarUrl: https://avatars.githubusercontent.com/u/39681546?u=5c028f81324b0e8c73b3c15bc4e7b0218d2ba0c3&v=4
     url: https://github.com/arleybri18
+  - login: thenickben
+    avatarUrl: https://avatars.githubusercontent.com/u/40610922?u=1e907d904041b7c91213951a3cb344cd37c14aaf&v=4
+    url: https://github.com/thenickben
   - login: ybressler
     avatarUrl: https://avatars.githubusercontent.com/u/40807730?u=41e2c00f1eebe3c402635f0325e41b4e6511462c&v=4
     url: https://github.com/ybressler
   - login: ddilidili
     avatarUrl: https://avatars.githubusercontent.com/u/42176885?u=c0a849dde06987434653197b5f638d3deb55fc6c&v=4
     url: https://github.com/ddilidili
-  - login: VictorCalderon
-    avatarUrl: https://avatars.githubusercontent.com/u/44529243?u=cea69884f826a29aff1415493405209e0706d07a&v=4
-    url: https://github.com/VictorCalderon
-  - login: rafsaf
-    avatarUrl: https://avatars.githubusercontent.com/u/51059348?u=f8f0d6d6e90fac39fa786228158ba7f013c74271&v=4
-    url: https://github.com/rafsaf
   - login: dudikbender
     avatarUrl: https://avatars.githubusercontent.com/u/53487583?u=3a57542938ebfd57579a0111db2b297e606d9681&v=4
     url: https://github.com/dudikbender
   - login: thisistheplace
     avatarUrl: https://avatars.githubusercontent.com/u/57633545?u=a3f3a7f8ace8511c6c067753f6eb6aee0db11ac6&v=4
     url: https://github.com/thisistheplace
-  - login: kyjoconn
-    avatarUrl: https://avatars.githubusercontent.com/u/58443406?u=a3e9c2acfb7ba62edda9334aba61cf027f41f789&v=4
-    url: https://github.com/kyjoconn
   - login: A-Edge
     avatarUrl: https://avatars.githubusercontent.com/u/59514131?v=4
     url: https://github.com/A-Edge
   - login: yakkonaut
     avatarUrl: https://avatars.githubusercontent.com/u/60633704?u=90a71fd631aa998ba4a96480788f017c9904e07b&v=4
     url: https://github.com/yakkonaut
   - login: patsatsia
     avatarUrl: https://avatars.githubusercontent.com/u/61111267?u=3271b85f7a37b479c8d0ae0a235182e83c166edf&v=4
     url: https://github.com/patsatsia
-  - login: predictionmachine
-    avatarUrl: https://avatars.githubusercontent.com/u/63719559?v=4
-    url: https://github.com/predictionmachine
   - login: daverin
     avatarUrl: https://avatars.githubusercontent.com/u/70378377?u=6d1814195c0de7162820eaad95a25b423a3869c0&v=4
     url: https://github.com/daverin
   - login: anthonycepeda
     avatarUrl: https://avatars.githubusercontent.com/u/72019805?u=4252c6b6dc5024af502a823a3ac5e7a03a69963f&v=4
     url: https://github.com/anthonycepeda
   - login: DelfinaCare
@@ -337,32 +280,29 @@
     url: https://github.com/osawa-koki
   - login: pyt3h
     avatarUrl: https://avatars.githubusercontent.com/u/99658549?v=4
     url: https://github.com/pyt3h
   - login: Dagmaara
     avatarUrl: https://avatars.githubusercontent.com/u/115501964?v=4
     url: https://github.com/Dagmaara
+- - login: Yarden-zamir
+    avatarUrl: https://avatars.githubusercontent.com/u/8178413?u=ee177a8b0f87ea56747f4d96f34cd4e9604a8217&v=4
+    url: https://github.com/Yarden-zamir
 - - login: pawamoy
     avatarUrl: https://avatars.githubusercontent.com/u/3999221?u=b030e4c89df2f3a36bc4710b925bdeb6745c9856&v=4
     url: https://github.com/pawamoy
-  - login: linux-china
-    avatarUrl: https://avatars.githubusercontent.com/u/46711?u=cd77c65338b158750eb84dc7ff1acf3209ccfc4f&v=4
-    url: https://github.com/linux-china
   - login: ddanier
     avatarUrl: https://avatars.githubusercontent.com/u/113563?u=ed1dc79de72f93bd78581f88ebc6952b62f472da&v=4
     url: https://github.com/ddanier
-  - login: jhb
-    avatarUrl: https://avatars.githubusercontent.com/u/142217?v=4
-    url: https://github.com/jhb
-  - login: justinrmiller
-    avatarUrl: https://avatars.githubusercontent.com/u/143998?u=b507a940394d4fc2bc1c27cea2ca9c22538874bd&v=4
-    url: https://github.com/justinrmiller
   - login: bryanculbertson
     avatarUrl: https://avatars.githubusercontent.com/u/144028?u=defda4f90e93429221cc667500944abde60ebe4a&v=4
     url: https://github.com/bryanculbertson
+  - login: slafs
+    avatarUrl: https://avatars.githubusercontent.com/u/210173?v=4
+    url: https://github.com/slafs
   - login: adamghill
     avatarUrl: https://avatars.githubusercontent.com/u/317045?u=f1349d5ffe84a19f324e204777859fbf69ddf633&v=4
     url: https://github.com/adamghill
   - login: eteq
     avatarUrl: https://avatars.githubusercontent.com/u/346587?v=4
     url: https://github.com/eteq
   - login: dmig
@@ -374,76 +314,88 @@
   - login: hardbyte
     avatarUrl: https://avatars.githubusercontent.com/u/855189?u=aa29e92f34708814d6b67fcd47ca4cf2ce1c04ed&v=4
     url: https://github.com/hardbyte
   - login: browniebroke
     avatarUrl: https://avatars.githubusercontent.com/u/861044?u=5abfca5588f3e906b31583d7ee62f6de4b68aa24&v=4
     url: https://github.com/browniebroke
   - login: janfilips
-    avatarUrl: https://avatars.githubusercontent.com/u/870699?u=50de77b93d3a0b06887e672d4e8c7b9d643085aa&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/870699?u=96df18ad355e58b9397accc55f4eeb7a86e959b0&v=4
     url: https://github.com/janfilips
-  - login: allen0125
-    avatarUrl: https://avatars.githubusercontent.com/u/1448456?u=dc2ad819497eef494b88688a1796e0adb87e7cae&v=4
-    url: https://github.com/allen0125
   - login: WillHogan
     avatarUrl: https://avatars.githubusercontent.com/u/1661551?u=7036c064cf29781470573865264ec8e60b6b809f&v=4
     url: https://github.com/WillHogan
   - login: my3
     avatarUrl: https://avatars.githubusercontent.com/u/1825270?v=4
     url: https://github.com/my3
   - login: cbonoz
     avatarUrl: https://avatars.githubusercontent.com/u/2351087?u=fd3e8030b2cc9fbfbb54a65e9890c548a016f58b&v=4
     url: https://github.com/cbonoz
-  - login: paul121
-    avatarUrl: https://avatars.githubusercontent.com/u/3116995?u=6e2d8691cc345e63ee02e4eb4d7cef82b1fcbedc&v=4
-    url: https://github.com/paul121
+  - login: Patechoc
+    avatarUrl: https://avatars.githubusercontent.com/u/2376641?u=23b49e9eda04f078cb74fa3f93593aa6a57bb138&v=4
+    url: https://github.com/Patechoc
   - login: larsvik
     avatarUrl: https://avatars.githubusercontent.com/u/3442226?v=4
     url: https://github.com/larsvik
   - login: anthonycorletti
     avatarUrl: https://avatars.githubusercontent.com/u/3477132?v=4
     url: https://github.com/anthonycorletti
+  - login: jonathanhle
+    avatarUrl: https://avatars.githubusercontent.com/u/3851599?u=76b9c5d2fecd6c3a16e7645231878c4507380d4d&v=4
+    url: https://github.com/jonathanhle
   - login: nikeee
-    avatarUrl: https://avatars.githubusercontent.com/u/4068864?u=63f8eee593f25138e0f1032ef442e9ad24907d4c&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/4068864?u=bbe73151f2b409c120160d032dc9aa6875ef0c4b&v=4
     url: https://github.com/nikeee
   - login: Alisa-lisa
     avatarUrl: https://avatars.githubusercontent.com/u/4137964?u=e7e393504f554f4ff15863a1e01a5746863ef9ce&v=4
     url: https://github.com/Alisa-lisa
   - login: danielunderwood
     avatarUrl: https://avatars.githubusercontent.com/u/4472301?v=4
     url: https://github.com/danielunderwood
+  - login: yuawn
+    avatarUrl: https://avatars.githubusercontent.com/u/5111198?u=5315576f3fe1a70fd2d0f02181588f4eea5d353d&v=4
+    url: https://github.com/yuawn
+  - login: sdevkota
+    avatarUrl: https://avatars.githubusercontent.com/u/5250987?u=4ed9a120c89805a8aefda1cbdc0cf6512e64d1b4&v=4
+    url: https://github.com/sdevkota
   - login: unredundant
     avatarUrl: https://avatars.githubusercontent.com/u/5607577?u=1ffbf39f5bb8736b75c0d235707d6e8f803725c5&v=4
     url: https://github.com/unredundant
   - login: Baghdady92
     avatarUrl: https://avatars.githubusercontent.com/u/5708590?v=4
     url: https://github.com/Baghdady92
   - login: KentShikama
     avatarUrl: https://avatars.githubusercontent.com/u/6329898?u=8b236810db9b96333230430837e1f021f9246da1&v=4
     url: https://github.com/KentShikama
-  - login: holec
-    avatarUrl: https://avatars.githubusercontent.com/u/6438041?u=f5af71ec85b3a9d7b8139cb5af0512b02fa9ab1e&v=4
-    url: https://github.com/holec
+  - login: katnoria
+    avatarUrl: https://avatars.githubusercontent.com/u/7674948?u=09767eb13e07e09496c5fee4e5ce21d9eac34a56&v=4
+    url: https://github.com/katnoria
   - login: mattwelke
-    avatarUrl: https://avatars.githubusercontent.com/u/7719209?v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/7719209?u=80f02a799323b1472b389b836d95957c93a6d856&v=4
     url: https://github.com/mattwelke
   - login: hcristea
     avatarUrl: https://avatars.githubusercontent.com/u/7814406?u=61d7a4fcf846983a4606788eac25e1c6c1209ba8&v=4
     url: https://github.com/hcristea
   - login: moonape1226
     avatarUrl: https://avatars.githubusercontent.com/u/8532038?u=d9f8b855a429fff9397c3833c2ff83849ebf989d&v=4
     url: https://github.com/moonape1226
+  - login: albertkun
+    avatarUrl: https://avatars.githubusercontent.com/u/8574425?u=aad2a9674273c9275fe414d99269b7418d144089&v=4
+    url: https://github.com/albertkun
   - login: xncbf
     avatarUrl: https://avatars.githubusercontent.com/u/9462045?u=866a1311e4bd3ec5ae84185c4fcc99f397c883d7&v=4
     url: https://github.com/xncbf
   - login: DMantis
     avatarUrl: https://avatars.githubusercontent.com/u/9536869?v=4
     url: https://github.com/DMantis
   - login: hard-coders
     avatarUrl: https://avatars.githubusercontent.com/u/9651103?u=95db33927bbff1ed1c07efddeb97ac2ff33068ed&v=4
     url: https://github.com/hard-coders
+  - login: supdann
+    avatarUrl: https://avatars.githubusercontent.com/u/9986994?u=9671810f4ae9504c063227fee34fd47567ff6954&v=4
+    url: https://github.com/supdann
   - login: satwikkansal
     avatarUrl: https://avatars.githubusercontent.com/u/10217535?u=b12d6ef74ea297de9e46da6933b1a5b7ba9e6a61&v=4
     url: https://github.com/satwikkansal
   - login: mntolia
     avatarUrl: https://avatars.githubusercontent.com/u/10390224?v=4
     url: https://github.com/mntolia
   - login: pheanex
@@ -452,96 +404,93 @@
   - login: JimFawkes
     avatarUrl: https://avatars.githubusercontent.com/u/12075115?u=dc58ecfd064d72887c34bf500ddfd52592509acd&v=4
     url: https://github.com/JimFawkes
   - login: giuliano-oliveira
     avatarUrl: https://avatars.githubusercontent.com/u/13181797?u=0ef2dfbf7fc9a9726d45c21d32b5d1038a174870&v=4
     url: https://github.com/giuliano-oliveira
   - login: TheR1D
-    avatarUrl: https://avatars.githubusercontent.com/u/16740832?u=b2923ac17fe6e2a7c9ea14800351ddb92f79b100&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/16740832?u=b0dfdbdb27b79729430c71c6128962f77b7b53f7&v=4
     url: https://github.com/TheR1D
-  - login: cdsre
-    avatarUrl: https://avatars.githubusercontent.com/u/16945936?v=4
-    url: https://github.com/cdsre
   - login: jangia
     avatarUrl: https://avatars.githubusercontent.com/u/17927101?u=9261b9bb0c3e3bb1ecba43e8915dc58d8c9a077e&v=4
     url: https://github.com/jangia
-  - login: paulowiz
-    avatarUrl: https://avatars.githubusercontent.com/u/18649504?u=d8a6ac40321f2bded0eba78b637751c7f86c6823&v=4
-    url: https://github.com/paulowiz
   - login: ghandic
     avatarUrl: https://avatars.githubusercontent.com/u/23500353?u=e2e1d736f924d9be81e8bfc565b6d8836ba99773&v=4
     url: https://github.com/ghandic
   - login: pers0n4
     avatarUrl: https://avatars.githubusercontent.com/u/24864600?u=f211a13a7b572cbbd7779b9c8d8cb428cc7ba07e&v=4
     url: https://github.com/pers0n4
-  - login: SebTota
-    avatarUrl: https://avatars.githubusercontent.com/u/25122511?v=4
-    url: https://github.com/SebTota
+  - login: kadekillary
+    avatarUrl: https://avatars.githubusercontent.com/u/25046261?u=e185e58080090f9e678192cd214a14b14a2b232b&v=4
+    url: https://github.com/kadekillary
   - login: hoenie-ams
     avatarUrl: https://avatars.githubusercontent.com/u/25708487?u=cda07434f0509ac728d9edf5e681117c0f6b818b&v=4
     url: https://github.com/hoenie-ams
   - login: joerambo
     avatarUrl: https://avatars.githubusercontent.com/u/26282974?v=4
     url: https://github.com/joerambo
+  - login: rlnchow
+    avatarUrl: https://avatars.githubusercontent.com/u/28018479?u=a93ca9cf1422b9ece155784a72d5f2fdbce7adff&v=4
+    url: https://github.com/rlnchow
   - login: mertguvencli
     avatarUrl: https://avatars.githubusercontent.com/u/29762151?u=16a906d90df96c8cff9ea131a575c4bc171b1523&v=4
     url: https://github.com/mertguvencli
-  - login: ruizdiazever
-    avatarUrl: https://avatars.githubusercontent.com/u/29817086?u=2df54af55663d246e3a4dc8273711c37f1adb117&v=4
-    url: https://github.com/ruizdiazever
   - login: HosamAlmoghraby
     avatarUrl: https://avatars.githubusercontent.com/u/32025281?u=aa1b09feabccbf9dc506b81c71155f32d126cefa&v=4
     url: https://github.com/HosamAlmoghraby
   - login: engineerjoe440
     avatarUrl: https://avatars.githubusercontent.com/u/33275230?u=eb223cad27017bb1e936ee9b429b450d092d0236&v=4
     url: https://github.com/engineerjoe440
   - login: bnkc
-    avatarUrl: https://avatars.githubusercontent.com/u/34930566?u=76cdc0a8b4e88c7d3e58dccb4b2670839e1247b4&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/34930566?u=9fbf76b9bf7786275e2900efa51d1394bcf1f06a&v=4
     url: https://github.com/bnkc
   - login: declon
     avatarUrl: https://avatars.githubusercontent.com/u/36180226?v=4
     url: https://github.com/declon
-  - login: alvarobartt
-    avatarUrl: https://avatars.githubusercontent.com/u/36760800?u=9b38695807eb981d452989699ff72ec2d8f6508e&v=4
-    url: https://github.com/alvarobartt
-  - login: d-e-h-i-o
-    avatarUrl: https://avatars.githubusercontent.com/u/36816716?v=4
-    url: https://github.com/d-e-h-i-o
-  - login: ww-daniel-mora
-    avatarUrl: https://avatars.githubusercontent.com/u/38921751?u=ae14bc1e40f2dd5a9c5741fc0b0dffbd416a5fa9&v=4
-    url: https://github.com/ww-daniel-mora
-  - login: rwxd
-    avatarUrl: https://avatars.githubusercontent.com/u/40308458?u=cd04a39e3655923be4f25c2ba8a5a07b3da3230a&v=4
-    url: https://github.com/rwxd
+  - login: miraedbswo
+    avatarUrl: https://avatars.githubusercontent.com/u/36796047?u=9e7a5b3e558edc61d35d0f9dfac37541bae7f56d&v=4
+    url: https://github.com/miraedbswo
+  - login: kristiangronberg
+    avatarUrl: https://avatars.githubusercontent.com/u/42678548?v=4
+    url: https://github.com/kristiangronberg
   - login: arrrrrmin
-    avatarUrl: https://avatars.githubusercontent.com/u/43553423?u=5265858add14a6822bd145f7547323cf078563e6&v=4
+    avatarUrl: https://avatars.githubusercontent.com/u/43553423?u=36a3880a6eb29309c19e6cadbb173bafbe91deb1&v=4
     url: https://github.com/arrrrrmin
+  - login: ArtyomVancyan
+    avatarUrl: https://avatars.githubusercontent.com/u/44609997?v=4
+    url: https://github.com/ArtyomVancyan
   - login: hgalytoby
     avatarUrl: https://avatars.githubusercontent.com/u/50397689?u=f4888c2c54929bd86eed0d3971d09fcb306e5088&v=4
     url: https://github.com/hgalytoby
-  - login: data-djinn
-    avatarUrl: https://avatars.githubusercontent.com/u/56449985?u=42146e140806908d49bd59ccc96f222abf587886&v=4
-    url: https://github.com/data-djinn
+  - login: eladgunders
+    avatarUrl: https://avatars.githubusercontent.com/u/52347338?u=83d454817cf991a035c8827d46ade050c813e2d6&v=4
+    url: https://github.com/eladgunders
+  - login: conservative-dude
+    avatarUrl: https://avatars.githubusercontent.com/u/55538308?u=f250c44942ea6e73a6bd90739b381c470c192c11&v=4
+    url: https://github.com/conservative-dude
   - login: leo-jp-edwards
     avatarUrl: https://avatars.githubusercontent.com/u/58213433?u=2c128e8b0794b7a66211cd7d8ebe05db20b7e9c0&v=4
     url: https://github.com/leo-jp-edwards
-  - login: apar-tiwari
-    avatarUrl: https://avatars.githubusercontent.com/u/61064197?v=4
-    url: https://github.com/apar-tiwari
-  - login: Vyvy-vi
-    avatarUrl: https://avatars.githubusercontent.com/u/62864373?u=1a9b0b28779abc2bc9b62cb4d2e44d453973c9c3&v=4
-    url: https://github.com/Vyvy-vi
+  - login: tamtam-fitness
+    avatarUrl: https://avatars.githubusercontent.com/u/62091034?u=8da19a6bd3d02f5d6ba30c7247d5b46c98dd1403&v=4
+    url: https://github.com/tamtam-fitness
   - login: 0417taehyun
     avatarUrl: https://avatars.githubusercontent.com/u/63915557?u=47debaa860fd52c9b98c97ef357ddcec3b3fb399&v=4
     url: https://github.com/0417taehyun
-  - login: realabja
-    avatarUrl: https://avatars.githubusercontent.com/u/66185192?u=001e2dd9297784f4218997981b4e6fa8357bb70b&v=4
-    url: https://github.com/realabja
-  - login: garydsong
-    avatarUrl: https://avatars.githubusercontent.com/u/105745865?u=03cc1aa9c978be0020e5a1ce1ecca323dd6c8d65&v=4
-    url: https://github.com/garydsong
-- - login: Leon0824
-    avatarUrl: https://avatars.githubusercontent.com/u/1922026?v=4
-    url: https://github.com/Leon0824
+- - login: ssbarnea
+    avatarUrl: https://avatars.githubusercontent.com/u/102495?u=b4bf6818deefe59952ac22fec6ed8c76de1b8f7c&v=4
+    url: https://github.com/ssbarnea
+  - login: sadikkuzu
+    avatarUrl: https://avatars.githubusercontent.com/u/23168063?u=d179c06bb9f65c4167fcab118526819f8e0dac17&v=4
+    url: https://github.com/sadikkuzu
+  - login: ruizdiazever
+    avatarUrl: https://avatars.githubusercontent.com/u/29817086?u=2df54af55663d246e3a4dc8273711c37f1adb117&v=4
+    url: https://github.com/ruizdiazever
   - login: danburonline
     avatarUrl: https://avatars.githubusercontent.com/u/34251194?u=2cad4388c1544e539ecb732d656e42fb07b4ff2d&v=4
     url: https://github.com/danburonline
+  - login: rwxd
+    avatarUrl: https://avatars.githubusercontent.com/u/40308458?u=cd04a39e3655923be4f25c2ba8a5a07b3da3230a&v=4
+    url: https://github.com/rwxd
+  - login: xNykram
+    avatarUrl: https://avatars.githubusercontent.com/u/55030025?u=2c1ba313fd79d29273b5ff7c9c5cf4edfb271b29&v=4
+    url: https://github.com/xNykram
```

### Comparing `fastapi-0.95.2/docs/en/data/people.yml` & `fastapi-0.96.0/docs/en/data/people.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 maintainers:
 - login: tiangolo
-  answers: 1827
-  prs: 384
+  answers: 1839
+  prs: 398
   avatarUrl: https://avatars.githubusercontent.com/u/1326112?u=740f11212a731f56798f558ceddb0bd07642afa7&v=4
   url: https://github.com/tiangolo
 experts:
 - login: Kludex
-  count: 376
+  count: 410
   avatarUrl: https://avatars.githubusercontent.com/u/7353520?u=62adc405ef418f4b6c8caa93d3eb8ab107bc4927&v=4
   url: https://github.com/Kludex
 - login: dmontagu
   count: 237
   avatarUrl: https://avatars.githubusercontent.com/u/35119617?u=58ed2a45798a4339700e2f62b2e12e6e54bf0396&v=4
   url: https://github.com/dmontagu
 - login: Mause
@@ -18,95 +18,95 @@
   avatarUrl: https://avatars.githubusercontent.com/u/1405026?v=4
   url: https://github.com/Mause
 - login: ycd
   count: 217
   avatarUrl: https://avatars.githubusercontent.com/u/62724709?u=bba5af018423a2858d49309bed2a899bb5c34ac5&v=4
   url: https://github.com/ycd
 - login: JarroVGIT
-  count: 192
+  count: 193
   avatarUrl: https://avatars.githubusercontent.com/u/13659033?u=e8bea32d07a5ef72f7dde3b2079ceb714923ca05&v=4
   url: https://github.com/JarroVGIT
 - login: euri10
-  count: 151
+  count: 152
   avatarUrl: https://avatars.githubusercontent.com/u/1104190?u=321a2e953e6645a7d09b732786c7a8061e0f8a8b&v=4
   url: https://github.com/euri10
 - login: phy25
   count: 126
   avatarUrl: https://avatars.githubusercontent.com/u/331403?v=4
   url: https://github.com/phy25
-- login: iudeen
-  count: 116
-  avatarUrl: https://avatars.githubusercontent.com/u/10519440?u=2843b3303282bff8b212dcd4d9d6689452e4470c&v=4
-  url: https://github.com/iudeen
 - login: jgould22
-  count: 101
+  count: 124
   avatarUrl: https://avatars.githubusercontent.com/u/4335847?u=ed77f67e0bb069084639b24d812dbb2a2b1dc554&v=4
   url: https://github.com/jgould22
+- login: iudeen
+  count: 118
+  avatarUrl: https://avatars.githubusercontent.com/u/10519440?u=2843b3303282bff8b212dcd4d9d6689452e4470c&v=4
+  url: https://github.com/iudeen
 - login: raphaelauv
   count: 83
   avatarUrl: https://avatars.githubusercontent.com/u/10202690?u=e6f86f5c0c3026a15d6b51792fa3e532b12f1371&v=4
   url: https://github.com/raphaelauv
-- login: ArcLightSlavik
-  count: 71
-  avatarUrl: https://avatars.githubusercontent.com/u/31127044?u=b0f2c37142f4b762e41ad65dc49581813422bd71&v=4
-  url: https://github.com/ArcLightSlavik
 - login: ghandic
   count: 71
   avatarUrl: https://avatars.githubusercontent.com/u/23500353?u=e2e1d736f924d9be81e8bfc565b6d8836ba99773&v=4
   url: https://github.com/ghandic
+- login: ArcLightSlavik
+  count: 71
+  avatarUrl: https://avatars.githubusercontent.com/u/31127044?u=b0f2c37142f4b762e41ad65dc49581813422bd71&v=4
+  url: https://github.com/ArcLightSlavik
 - login: falkben
   count: 57
-  avatarUrl: https://avatars.githubusercontent.com/u/653031?u=0c8d8f33d87f1aa1a6488d3f02105e9abc838105&v=4
+  avatarUrl: https://avatars.githubusercontent.com/u/653031?u=ad9838e089058c9e5a0bab94c0eec7cc181e0cd0&v=4
   url: https://github.com/falkben
 - login: sm-Fifteen
   count: 49
   avatarUrl: https://avatars.githubusercontent.com/u/516999?u=437c0c5038558c67e887ccd863c1ba0f846c03da&v=4
   url: https://github.com/sm-Fifteen
-- login: Dustyposa
+- login: yinziyan1206
   count: 45
-  avatarUrl: https://avatars.githubusercontent.com/u/27180793?u=5cf2877f50b3eb2bc55086089a78a36f07042889&v=4
-  url: https://github.com/Dustyposa
+  avatarUrl: https://avatars.githubusercontent.com/u/37829370?u=da44ca53aefd5c23f346fab8e9fd2e108294c179&v=4
+  url: https://github.com/yinziyan1206
 - login: insomnes
   count: 45
   avatarUrl: https://avatars.githubusercontent.com/u/16958893?u=f8be7088d5076d963984a21f95f44e559192d912&v=4
   url: https://github.com/insomnes
+- login: acidjunk
+  count: 45
+  avatarUrl: https://avatars.githubusercontent.com/u/685002?u=b5094ab4527fc84b006c0ac9ff54367bdebb2267&v=4
+  url: https://github.com/acidjunk
+- login: Dustyposa
+  count: 45
+  avatarUrl: https://avatars.githubusercontent.com/u/27180793?u=5cf2877f50b3eb2bc55086089a78a36f07042889&v=4
+  url: https://github.com/Dustyposa
+- login: adriangb
+  count: 43
+  avatarUrl: https://avatars.githubusercontent.com/u/1755071?u=1e2c2c9b39f5c9b780fb933d8995cf08ec235a47&v=4
+  url: https://github.com/adriangb
 - login: frankie567
   count: 43
   avatarUrl: https://avatars.githubusercontent.com/u/1144727?u=85c025e3fcc7bd79a5665c63ee87cdf8aae13374&v=4
   url: https://github.com/frankie567
-- login: acidjunk
-  count: 43
-  avatarUrl: https://avatars.githubusercontent.com/u/685002?u=b5094ab4527fc84b006c0ac9ff54367bdebb2267&v=4
-  url: https://github.com/acidjunk
 - login: odiseo0
   count: 42
-  avatarUrl: https://avatars.githubusercontent.com/u/87550035?u=16f9255804161c6ff3c8b7ef69848f0126bcd405&v=4
+  avatarUrl: https://avatars.githubusercontent.com/u/87550035?u=2da05dab6cc8e1ade557801634760a56e4101796&v=4
   url: https://github.com/odiseo0
-- login: adriangb
-  count: 40
-  avatarUrl: https://avatars.githubusercontent.com/u/1755071?u=1e2c2c9b39f5c9b780fb933d8995cf08ec235a47&v=4
-  url: https://github.com/adriangb
 - login: includeamin
   count: 40
   avatarUrl: https://avatars.githubusercontent.com/u/11836741?u=8bd5ef7e62fe6a82055e33c4c0e0a7879ff8cfb6&v=4
   url: https://github.com/includeamin
 - login: STeveShary
   count: 37
   avatarUrl: https://avatars.githubusercontent.com/u/5167622?u=de8f597c81d6336fcebc37b32dfd61a3f877160c&v=4
   url: https://github.com/STeveShary
 - login: krishnardt
   count: 35
   avatarUrl: https://avatars.githubusercontent.com/u/31960541?u=47f4829c77f4962ab437ffb7995951e41eeebe9b&v=4
   url: https://github.com/krishnardt
-- login: yinziyan1206
-  count: 34
-  avatarUrl: https://avatars.githubusercontent.com/u/37829370?u=da44ca53aefd5c23f346fab8e9fd2e108294c179&v=4
-  url: https://github.com/yinziyan1206
 - login: chbndrhnns
-  count: 34
+  count: 35
   avatarUrl: https://avatars.githubusercontent.com/u/7534547?v=4
   url: https://github.com/chbndrhnns
 - login: panla
   count: 32
   avatarUrl: https://avatars.githubusercontent.com/u/41326348?u=ba2fda6b30110411ecbf406d187907e2b420ac19&v=4
   url: https://github.com/panla
 - login: prostomarkeloff
@@ -121,123 +121,111 @@
   count: 25
   avatarUrl: https://avatars.githubusercontent.com/u/365303?u=07ca03c5ee811eb0920e633cc3c3db73dbec1aa5&v=4
   url: https://github.com/wshayes
 - login: SirTelemak
   count: 23
   avatarUrl: https://avatars.githubusercontent.com/u/9435877?u=719327b7d2c4c62212456d771bfa7c6b8dbb9eac&v=4
   url: https://github.com/SirTelemak
-- login: caeser1996
-  count: 21
-  avatarUrl: https://avatars.githubusercontent.com/u/16540232?u=05d2beb8e034d584d0a374b99d8826327bd7f614&v=4
-  url: https://github.com/caeser1996
+- login: acnebs
+  count: 22
+  avatarUrl: https://avatars.githubusercontent.com/u/9054108?u=c27e50269f1ef8ea950cc6f0268c8ec5cebbe9c9&v=4
+  url: https://github.com/acnebs
 - login: rafsaf
   count: 21
   avatarUrl: https://avatars.githubusercontent.com/u/51059348?u=f8f0d6d6e90fac39fa786228158ba7f013c74271&v=4
   url: https://github.com/rafsaf
 - login: nsidnev
   count: 20
   avatarUrl: https://avatars.githubusercontent.com/u/22559461?u=a9cc3238217e21dc8796a1a500f01b722adb082c&v=4
   url: https://github.com/nsidnev
-- login: acnebs
-  count: 20
-  avatarUrl: https://avatars.githubusercontent.com/u/9054108?u=c27e50269f1ef8ea950cc6f0268c8ec5cebbe9c9&v=4
-  url: https://github.com/acnebs
 - login: chris-allnutt
   count: 20
   avatarUrl: https://avatars.githubusercontent.com/u/565544?v=4
   url: https://github.com/chris-allnutt
-- login: retnikt
-  count: 18
-  avatarUrl: https://avatars.githubusercontent.com/u/24581770?v=4
-  url: https://github.com/retnikt
 - login: zoliknemet
   count: 18
   avatarUrl: https://avatars.githubusercontent.com/u/22326718?u=31ba446ac290e23e56eea8e4f0c558aaf0b40779&v=4
   url: https://github.com/zoliknemet
-- login: nkhitrov
+- login: retnikt
+  count: 18
+  avatarUrl: https://avatars.githubusercontent.com/u/24581770?v=4
+  url: https://github.com/retnikt
+- login: Hultner
   count: 17
-  avatarUrl: https://avatars.githubusercontent.com/u/28262306?u=66ee21316275ef356081c2efc4ed7a4572e690dc&v=4
-  url: https://github.com/nkhitrov
+  avatarUrl: https://avatars.githubusercontent.com/u/2669034?u=115e53df959309898ad8dc9443fbb35fee71df07&v=4
+  url: https://github.com/Hultner
+- login: n8sty
+  count: 17
+  avatarUrl: https://avatars.githubusercontent.com/u/2964996?v=4
+  url: https://github.com/n8sty
 - login: harunyasar
   count: 17
   avatarUrl: https://avatars.githubusercontent.com/u/1765494?u=5b1ab7c582db4b4016fa31affe977d10af108ad4&v=4
   url: https://github.com/harunyasar
-- login: Hultner
+- login: nkhitrov
   count: 17
-  avatarUrl: https://avatars.githubusercontent.com/u/2669034?u=115e53df959309898ad8dc9443fbb35fee71df07&v=4
-  url: https://github.com/Hultner
+  avatarUrl: https://avatars.githubusercontent.com/u/28262306?u=66ee21316275ef356081c2efc4ed7a4572e690dc&v=4
+  url: https://github.com/nkhitrov
+- login: caeser1996
+  count: 17
+  avatarUrl: https://avatars.githubusercontent.com/u/16540232?u=05d2beb8e034d584d0a374b99d8826327bd7f614&v=4
+  url: https://github.com/caeser1996
 - login: jonatasoli
   count: 16
   avatarUrl: https://avatars.githubusercontent.com/u/26334101?u=071c062d2861d3dd127f6b4a5258cd8ef55d4c50&v=4
   url: https://github.com/jonatasoli
 - login: dstlny
   count: 16
   avatarUrl: https://avatars.githubusercontent.com/u/41964673?u=9f2174f9d61c15c6e3a4c9e3aeee66f711ce311f&v=4
   url: https://github.com/dstlny
-- login: jorgerpo
-  count: 15
-  avatarUrl: https://avatars.githubusercontent.com/u/12537771?u=7444d20019198e34911082780cc7ad73f2b97cb3&v=4
-  url: https://github.com/jorgerpo
 - login: ghost
   count: 15
   avatarUrl: https://avatars.githubusercontent.com/u/10137?u=b1951d34a583cf12ec0d3b0781ba19be97726318&v=4
   url: https://github.com/ghost
 - login: simondale00
   count: 15
   avatarUrl: https://avatars.githubusercontent.com/u/33907262?v=4
   url: https://github.com/simondale00
+- login: jorgerpo
+  count: 15
+  avatarUrl: https://avatars.githubusercontent.com/u/12537771?u=7444d20019198e34911082780cc7ad73f2b97cb3&v=4
+  url: https://github.com/jorgerpo
+- login: ebottos94
+  count: 14
+  avatarUrl: https://avatars.githubusercontent.com/u/100039558?u=e2c672da5a7977fd24d87ce6ab35f8bf5b1ed9fa&v=4
+  url: https://github.com/ebottos94
 - login: hellocoldworld
   count: 14
   avatarUrl: https://avatars.githubusercontent.com/u/47581948?u=3d2186796434c507a6cb6de35189ab0ad27c356f&v=4
   url: https://github.com/hellocoldworld
-- login: waynerv
-  count: 14
-  avatarUrl: https://avatars.githubusercontent.com/u/39515546?u=ec35139777597cdbbbddda29bf8b9d4396b429a9&v=4
-  url: https://github.com/waynerv
-- login: mbroton
-  count: 13
-  avatarUrl: https://avatars.githubusercontent.com/u/50829834?u=a48610bf1bffaa9c75d03228926e2eb08a2e24ee&v=4
-  url: https://github.com/mbroton
 last_month_active:
-- login: mr-st0rm
-  count: 7
-  avatarUrl: https://avatars.githubusercontent.com/u/48455163?u=6b83550e4e70bea57cd2fdb41e717aeab7f64a91&v=4
-  url: https://github.com/mr-st0rm
-- login: caeser1996
-  count: 7
-  avatarUrl: https://avatars.githubusercontent.com/u/16540232?u=05d2beb8e034d584d0a374b99d8826327bd7f614&v=4
-  url: https://github.com/caeser1996
-- login: ebottos94
-  count: 6
-  avatarUrl: https://avatars.githubusercontent.com/u/100039558?u=e2c672da5a7977fd24d87ce6ab35f8bf5b1ed9fa&v=4
-  url: https://github.com/ebottos94
 - login: jgould22
-  count: 6
+  count: 13
   avatarUrl: https://avatars.githubusercontent.com/u/4335847?u=ed77f67e0bb069084639b24d812dbb2a2b1dc554&v=4
   url: https://github.com/jgould22
 - login: Kludex
-  count: 5
+  count: 7
   avatarUrl: https://avatars.githubusercontent.com/u/7353520?u=62adc405ef418f4b6c8caa93d3eb8ab107bc4927&v=4
   url: https://github.com/Kludex
-- login: clemens-tolboom
+- login: abhint
+  count: 5
+  avatarUrl: https://avatars.githubusercontent.com/u/25699289?u=5b9f9f6192c83ca86a411eafd4be46d9e5828585&v=4
+  url: https://github.com/abhint
+- login: chrisK824
   count: 4
-  avatarUrl: https://avatars.githubusercontent.com/u/371014?v=4
-  url: https://github.com/clemens-tolboom
-- login: williamjamir
+  avatarUrl: https://avatars.githubusercontent.com/u/79946379?u=03d85b22d696a58a9603e55fbbbe2de6b0f4face&v=4
+  url: https://github.com/chrisK824
+- login: djimontyp
   count: 4
-  avatarUrl: https://avatars.githubusercontent.com/u/5083518?u=b76ca8e08b906a86fa195fb817dd94e8d9d3d8f6&v=4
-  url: https://github.com/williamjamir
-- login: nymous
-  count: 3
-  avatarUrl: https://avatars.githubusercontent.com/u/4216559?u=360a36fb602cded27273cbfc0afc296eece90662&v=4
-  url: https://github.com/nymous
-- login: frankie567
+  avatarUrl: https://avatars.githubusercontent.com/u/53098395?u=583bade70950b277c322d35f1be2b75c7b0f189c&v=4
+  url: https://github.com/djimontyp
+- login: JavierSanchezCastro
   count: 3
-  avatarUrl: https://avatars.githubusercontent.com/u/1144727?u=85c025e3fcc7bd79a5665c63ee87cdf8aae13374&v=4
-  url: https://github.com/frankie567
+  avatarUrl: https://avatars.githubusercontent.com/u/72013291?u=ae5679e6bd971d9d98cd5e76e8683f83642ba950&v=4
+  url: https://github.com/JavierSanchezCastro
 top_contributors:
 - login: waynerv
   count: 25
   avatarUrl: https://avatars.githubusercontent.com/u/39515546?u=ec35139777597cdbbbddda29bf8b9d4396b429a9&v=4
   url: https://github.com/waynerv
 - login: tokusumi
   count: 22
@@ -259,42 +247,50 @@
   count: 13
   avatarUrl: https://avatars.githubusercontent.com/u/1104190?u=321a2e953e6645a7d09b732786c7a8061e0f8a8b&v=4
   url: https://github.com/euri10
 - login: mariacamilagl
   count: 12
   avatarUrl: https://avatars.githubusercontent.com/u/11489395?u=4adb6986bf3debfc2b8216ae701f2bd47d73da7d&v=4
   url: https://github.com/mariacamilagl
+- login: Xewus
+  count: 12
+  avatarUrl: https://avatars.githubusercontent.com/u/85196001?u=f8e2dc7e5104f109cef944af79050ea8d1b8f914&v=4
+  url: https://github.com/Xewus
 - login: Smlep
   count: 10
   avatarUrl: https://avatars.githubusercontent.com/u/16785985?v=4
   url: https://github.com/Smlep
 - login: Serrones
   count: 8
   avatarUrl: https://avatars.githubusercontent.com/u/22691749?u=4795b880e13ca33a73e52fc0ef7dc9c60c8fce47&v=4
   url: https://github.com/Serrones
+- login: rjNemo
+  count: 8
+  avatarUrl: https://avatars.githubusercontent.com/u/56785022?u=d5c3a02567c8649e146fcfc51b6060ccaf8adef8&v=4
+  url: https://github.com/rjNemo
 - login: RunningIkkyu
   count: 7
   avatarUrl: https://avatars.githubusercontent.com/u/31848542?u=494ecc298e3f26197495bb357ad0f57cfd5f7a32&v=4
   url: https://github.com/RunningIkkyu
 - login: hard-coders
   count: 7
   avatarUrl: https://avatars.githubusercontent.com/u/9651103?u=95db33927bbff1ed1c07efddeb97ac2ff33068ed&v=4
   url: https://github.com/hard-coders
-- login: rjNemo
-  count: 7
-  avatarUrl: https://avatars.githubusercontent.com/u/56785022?u=d5c3a02567c8649e146fcfc51b6060ccaf8adef8&v=4
-  url: https://github.com/rjNemo
 - login: batlopes
   count: 6
   avatarUrl: https://avatars.githubusercontent.com/u/33462923?u=0fb3d7acb316764616f11e4947faf080e49ad8d9&v=4
   url: https://github.com/batlopes
 - login: wshayes
   count: 5
   avatarUrl: https://avatars.githubusercontent.com/u/365303?u=07ca03c5ee811eb0920e633cc3c3db73dbec1aa5&v=4
   url: https://github.com/wshayes
+- login: samuelcolvin
+  count: 5
+  avatarUrl: https://avatars.githubusercontent.com/u/4039449?u=807390ba9cfe23906c3bf8a0d56aaca3cf2bfa0d&v=4
+  url: https://github.com/samuelcolvin
 - login: SwftAlpc
   count: 5
   avatarUrl: https://avatars.githubusercontent.com/u/52768429?u=6a3aa15277406520ad37f6236e89466ed44bc5b8&v=4
   url: https://github.com/SwftAlpc
 - login: Attsun1031
   count: 5
   avatarUrl: https://avatars.githubusercontent.com/u/1175560?v=4
@@ -303,26 +299,18 @@
   count: 5
   avatarUrl: https://avatars.githubusercontent.com/u/43503750?u=f440bc9062afb3c43b9b9c6cdfdcfe31d58699ef&v=4
   url: https://github.com/ComicShrimp
 - login: NinaHwang
   count: 5
   avatarUrl: https://avatars.githubusercontent.com/u/79563565?u=eee6bfe9224c71193025ab7477f4f96ceaa05c62&v=4
   url: https://github.com/NinaHwang
-- login: Xewus
-  count: 5
-  avatarUrl: https://avatars.githubusercontent.com/u/85196001?u=f8e2dc7e5104f109cef944af79050ea8d1b8f914&v=4
-  url: https://github.com/Xewus
 - login: jekirl
   count: 4
   avatarUrl: https://avatars.githubusercontent.com/u/2546697?u=a027452387d85bd4a14834e19d716c99255fb3b7&v=4
   url: https://github.com/jekirl
-- login: samuelcolvin
-  count: 4
-  avatarUrl: https://avatars.githubusercontent.com/u/4039449?u=807390ba9cfe23906c3bf8a0d56aaca3cf2bfa0d&v=4
-  url: https://github.com/samuelcolvin
 - login: jfunez
   count: 4
   avatarUrl: https://avatars.githubusercontent.com/u/805749?v=4
   url: https://github.com/jfunez
 - login: ycd
   count: 4
   avatarUrl: https://avatars.githubusercontent.com/u/62724709?u=bba5af018423a2858d49309bed2a899bb5c34ac5&v=4
@@ -335,26 +323,30 @@
   count: 4
   avatarUrl: https://avatars.githubusercontent.com/u/3360631?u=5fa1f475ad784d64eb9666bdd43cc4d285dcc773&v=4
   url: https://github.com/hitrust
 - login: lsglucas
   count: 4
   avatarUrl: https://avatars.githubusercontent.com/u/61513630?u=320e43fe4dc7bc6efc64e9b8f325f8075634fd20&v=4
   url: https://github.com/lsglucas
+- login: axel584
+  count: 4
+  avatarUrl: https://avatars.githubusercontent.com/u/1334088?u=9667041f5b15dc002b6f9665fda8c0412933ac04&v=4
+  url: https://github.com/axel584
 top_reviewers:
 - login: Kludex
-  count: 111
+  count: 117
   avatarUrl: https://avatars.githubusercontent.com/u/7353520?u=62adc405ef418f4b6c8caa93d3eb8ab107bc4927&v=4
   url: https://github.com/Kludex
 - login: BilalAlpaslan
   count: 75
   avatarUrl: https://avatars.githubusercontent.com/u/47563997?u=63ed66e304fe8d765762c70587d61d9196e5c82d&v=4
   url: https://github.com/BilalAlpaslan
 - login: yezz123
-  count: 71
-  avatarUrl: https://avatars.githubusercontent.com/u/52716203?u=636b4f79645176df4527dd45c12d5dbb5a4193cf&v=4
+  count: 74
+  avatarUrl: https://avatars.githubusercontent.com/u/52716203?u=d7062cbc6eb7671d5dc9cc0e32a24ae335e0f225&v=4
   url: https://github.com/yezz123
 - login: tokusumi
   count: 51
   avatarUrl: https://avatars.githubusercontent.com/u/41147016?u=55010621aece725aa702270b54fed829b6a1fe60&v=4
   url: https://github.com/tokusumi
 - login: waynerv
   count: 47
@@ -380,14 +372,18 @@
   count: 34
   avatarUrl: https://avatars.githubusercontent.com/u/13659033?u=e8bea32d07a5ef72f7dde3b2079ceb714923ca05&v=4
   url: https://github.com/JarroVGIT
 - login: AdrianDeAnda
   count: 33
   avatarUrl: https://avatars.githubusercontent.com/u/1024932?u=b2ea249c6b41ddf98679c8d110d0f67d4a3ebf93&v=4
   url: https://github.com/AdrianDeAnda
+- login: Xewus
+  count: 32
+  avatarUrl: https://avatars.githubusercontent.com/u/85196001?u=f8e2dc7e5104f109cef944af79050ea8d1b8f914&v=4
+  url: https://github.com/Xewus
 - login: ArcLightSlavik
   count: 31
   avatarUrl: https://avatars.githubusercontent.com/u/31127044?u=b0f2c37142f4b762e41ad65dc49581813422bd71&v=4
   url: https://github.com/ArcLightSlavik
 - login: cassiobotaro
   count: 28
   avatarUrl: https://avatars.githubusercontent.com/u/3127847?u=b0a652331da17efeb85cd6e3a4969182e5004804&v=4
@@ -396,38 +392,42 @@
   count: 27
   avatarUrl: https://avatars.githubusercontent.com/u/39375566?u=260ad6b1a4b34c07dbfa728da5e586f16f6d1824&v=4
   url: https://github.com/komtaki
 - login: lsglucas
   count: 26
   avatarUrl: https://avatars.githubusercontent.com/u/61513630?u=320e43fe4dc7bc6efc64e9b8f325f8075634fd20&v=4
   url: https://github.com/lsglucas
+- login: Ryandaydev
+  count: 24
+  avatarUrl: https://avatars.githubusercontent.com/u/4292423?u=809f3d1074d04bbc28012a7f17f06ea56f5bd71a&v=4
+  url: https://github.com/Ryandaydev
 - login: dmontagu
   count: 23
   avatarUrl: https://avatars.githubusercontent.com/u/35119617?u=58ed2a45798a4339700e2f62b2e12e6e54bf0396&v=4
   url: https://github.com/dmontagu
 - login: LorhanSohaky
-  count: 22
+  count: 23
   avatarUrl: https://avatars.githubusercontent.com/u/16273730?u=095b66f243a2cd6a0aadba9a095009f8aaf18393&v=4
   url: https://github.com/LorhanSohaky
 - login: rjNemo
-  count: 20
+  count: 21
   avatarUrl: https://avatars.githubusercontent.com/u/56785022?u=d5c3a02567c8649e146fcfc51b6060ccaf8adef8&v=4
   url: https://github.com/rjNemo
 - login: hard-coders
-  count: 20
+  count: 21
   avatarUrl: https://avatars.githubusercontent.com/u/9651103?u=95db33927bbff1ed1c07efddeb97ac2ff33068ed&v=4
   url: https://github.com/hard-coders
+- login: odiseo0
+  count: 20
+  avatarUrl: https://avatars.githubusercontent.com/u/87550035?u=2da05dab6cc8e1ade557801634760a56e4101796&v=4
+  url: https://github.com/odiseo0
 - login: 0417taehyun
   count: 19
   avatarUrl: https://avatars.githubusercontent.com/u/63915557?u=47debaa860fd52c9b98c97ef357ddcec3b3fb399&v=4
   url: https://github.com/0417taehyun
-- login: odiseo0
-  count: 19
-  avatarUrl: https://avatars.githubusercontent.com/u/87550035?u=16f9255804161c6ff3c8b7ef69848f0126bcd405&v=4
-  url: https://github.com/odiseo0
 - login: Smlep
   count: 17
   avatarUrl: https://avatars.githubusercontent.com/u/16785985?v=4
   url: https://github.com/Smlep
 - login: zy7y
   count: 17
   avatarUrl: https://avatars.githubusercontent.com/u/67154681?u=5d634834cc514028ea3f9115f7030b99a1f4d5a4&v=4
@@ -448,58 +448,62 @@
   count: 15
   avatarUrl: https://avatars.githubusercontent.com/u/16860088?u=abf922a7b920bf8fdb7867d8b43e091f1e796178&v=4
   url: https://github.com/pedabraham
 - login: delhi09
   count: 15
   avatarUrl: https://avatars.githubusercontent.com/u/63476957?u=6c86e59b48e0394d4db230f37fc9ad4d7e2c27c7&v=4
   url: https://github.com/delhi09
-- login: Ryandaydev
-  count: 15
-  avatarUrl: https://avatars.githubusercontent.com/u/4292423?u=809f3d1074d04bbc28012a7f17f06ea56f5bd71a&v=4
-  url: https://github.com/Ryandaydev
-- login: Xewus
-  count: 14
-  avatarUrl: https://avatars.githubusercontent.com/u/85196001?u=f8e2dc7e5104f109cef944af79050ea8d1b8f914&v=4
-  url: https://github.com/Xewus
 - login: sh0nk
   count: 13
   avatarUrl: https://avatars.githubusercontent.com/u/6478810?u=af15d724875cec682ed8088a86d36b2798f981c0&v=4
   url: https://github.com/sh0nk
 - login: peidrao
   count: 13
-  avatarUrl: https://avatars.githubusercontent.com/u/32584628?u=5401640e0b961cc199dee39ec79e162c7833cd6b&v=4
+  avatarUrl: https://avatars.githubusercontent.com/u/32584628?u=5b94b548ef0002ef3219d7c07ac0fac17c6201a2&v=4
   url: https://github.com/peidrao
+- login: r0b2g1t
+  count: 13
+  avatarUrl: https://avatars.githubusercontent.com/u/5357541?u=6428442d875d5d71aaa1bb38bb11c4be1a526bc2&v=4
+  url: https://github.com/r0b2g1t
 - login: RunningIkkyu
   count: 12
   avatarUrl: https://avatars.githubusercontent.com/u/31848542?u=494ecc298e3f26197495bb357ad0f57cfd5f7a32&v=4
   url: https://github.com/RunningIkkyu
+- login: axel584
+  count: 12
+  avatarUrl: https://avatars.githubusercontent.com/u/1334088?u=9667041f5b15dc002b6f9665fda8c0412933ac04&v=4
+  url: https://github.com/axel584
 - login: solomein-sv
   count: 11
-  avatarUrl: https://avatars.githubusercontent.com/u/46193920?u=46acfb4aeefb1d7b9fdc5a8cbd9eb8744683c47a&v=4
+  avatarUrl: https://avatars.githubusercontent.com/u/46193920?u=789927ee09cfabd752d3bd554fa6baf4850d2777&v=4
   url: https://github.com/solomein-sv
 - login: mariacamilagl
   count: 10
   avatarUrl: https://avatars.githubusercontent.com/u/11489395?u=4adb6986bf3debfc2b8216ae701f2bd47d73da7d&v=4
   url: https://github.com/mariacamilagl
+- login: raphaelauv
+  count: 10
+  avatarUrl: https://avatars.githubusercontent.com/u/10202690?u=e6f86f5c0c3026a15d6b51792fa3e532b12f1371&v=4
+  url: https://github.com/raphaelauv
 - login: Attsun1031
   count: 10
   avatarUrl: https://avatars.githubusercontent.com/u/1175560?v=4
   url: https://github.com/Attsun1031
 - login: maoyibo
   count: 10
   avatarUrl: https://avatars.githubusercontent.com/u/7887703?v=4
   url: https://github.com/maoyibo
 - login: ComicShrimp
   count: 10
   avatarUrl: https://avatars.githubusercontent.com/u/43503750?u=f440bc9062afb3c43b9b9c6cdfdcfe31d58699ef&v=4
   url: https://github.com/ComicShrimp
-- login: r0b2g1t
+- login: Alexandrhub
   count: 10
-  avatarUrl: https://avatars.githubusercontent.com/u/5357541?u=6428442d875d5d71aaa1bb38bb11c4be1a526bc2&v=4
-  url: https://github.com/r0b2g1t
+  avatarUrl: https://avatars.githubusercontent.com/u/119126536?u=9fc0d48f3307817bafecc5861eb2168401a6cb04&v=4
+  url: https://github.com/Alexandrhub
 - login: izaguerreiro
   count: 9
   avatarUrl: https://avatars.githubusercontent.com/u/2241504?v=4
   url: https://github.com/izaguerreiro
 - login: graingert
   count: 9
   avatarUrl: https://avatars.githubusercontent.com/u/413772?u=64b77b6aa405c68a9c6bcf45f84257c66eea5f32&v=4
@@ -512,27 +516,15 @@
   count: 9
   avatarUrl: https://avatars.githubusercontent.com/u/49435654?v=4
   url: https://github.com/kty4119
 - login: bezaca
   count: 9
   avatarUrl: https://avatars.githubusercontent.com/u/69092910?u=4ac58eab99bd37d663f3d23551df96d4fbdbf760&v=4
   url: https://github.com/bezaca
-- login: dimaqq
+- login: oandersonmagalhaes
   count: 9
-  avatarUrl: https://avatars.githubusercontent.com/u/662249?v=4
-  url: https://github.com/dimaqq
-- login: raphaelauv
-  count: 8
-  avatarUrl: https://avatars.githubusercontent.com/u/10202690?u=e6f86f5c0c3026a15d6b51792fa3e532b12f1371&v=4
-  url: https://github.com/raphaelauv
-- login: axel584
-  count: 8
-  avatarUrl: https://avatars.githubusercontent.com/u/1334088?v=4
-  url: https://github.com/axel584
-- login: blt232018
-  count: 8
-  avatarUrl: https://avatars.githubusercontent.com/u/43393471?u=172b0e0391db1aa6c1706498d6dfcb003c8a4857&v=4
-  url: https://github.com/blt232018
-- login: rogerbrinkmann
-  count: 8
-  avatarUrl: https://avatars.githubusercontent.com/u/5690226?v=4
-  url: https://github.com/rogerbrinkmann
+  avatarUrl: https://avatars.githubusercontent.com/u/83456692?v=4
+  url: https://github.com/oandersonmagalhaes
+- login: NinaHwang
+  count: 9
+  avatarUrl: https://avatars.githubusercontent.com/u/79563565?u=eee6bfe9224c71193025ab7477f4f96ceaa05c62&v=4
+  url: https://github.com/NinaHwang
```

### Comparing `fastapi-0.95.2/docs/en/data/sponsors.yml` & `fastapi-0.96.0/docs/en/data/sponsors.yml`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,14 @@
   - url: https://cryptapi.io/
     title: "CryptAPI: Your easy to use, secure and privacy oriented payment gateway."
     img: https://fastapi.tiangolo.com/img/sponsors/cryptapi.svg
 silver:
   - url: https://www.deta.sh/?ref=fastapi
     title: The launchpad for all your (team's) ideas
     img: https://fastapi.tiangolo.com/img/sponsors/deta.svg
-  - url: https://www.investsuite.com/jobs
-    title: Wealthtech jobs with FastAPI
-    img: https://fastapi.tiangolo.com/img/sponsors/investsuite.svg
   - url: https://training.talkpython.fm/fastapi-courses
     title: FastAPI video courses on demand from people you trust
     img: https://fastapi.tiangolo.com/img/sponsors/talkpython.png
   - url: https://testdriven.io/courses/tdd-fastapi/
     title: Learn to build high-quality web apps with best practices
     img: https://fastapi.tiangolo.com/img/sponsors/testdriven.svg
   - url: https://github.com/deepset-ai/haystack/
```

### Comparing `fastapi-0.95.2/docs/en/docs/alternatives.md` & `fastapi-0.96.0/docs/en/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/async.md` & `fastapi-0.96.0/docs/en/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/benchmarks.md` & `fastapi-0.96.0/docs/en/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/contributing.md` & `fastapi-0.96.0/docs/en/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/external-links.md` & `fastapi-0.96.0/docs/en/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/fastapi-people.md` & `fastapi-0.96.0/docs/en/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/features.md` & `fastapi-0.96.0/docs/en/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/help-fastapi.md` & `fastapi-0.96.0/docs/en/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/history-design-future.md` & `fastapi-0.96.0/docs/en/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/index.md` & `fastapi-0.96.0/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/project-generation.md` & `fastapi-0.96.0/docs/en/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/python-types.md` & `fastapi-0.96.0/docs/en/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/release-notes.md` & `fastapi-0.96.0/docs/en/docs/release-notes.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 # Release Notes
 
 ## Latest Changes
 
 
+## 0.96.0
+
+### Features
+
+* ⚡ Update `create_cloned_field` to use a global cache and improve startup performance. PR [#4645](https://github.com/tiangolo/fastapi/pull/4645) by [@madkinsz](https://github.com/madkinsz) and previous original PR by [@huonw](https://github.com/huonw).
+
+### Docs
+
+* 📝 Update Deta deployment tutorial for compatibility with Deta Space. PR [#6004](https://github.com/tiangolo/fastapi/pull/6004) by [@mikBighne98](https://github.com/mikBighne98).
+* ✏️ Fix typo in Deta deployment tutorial. PR [#9501](https://github.com/tiangolo/fastapi/pull/9501) by [@lemonyte](https://github.com/lemonyte).
+
+### Translations
+
+* 🌐 Add Russian translation for `docs/tutorial/body.md`. PR [#3885](https://github.com/tiangolo/fastapi/pull/3885) by [@solomein-sv](https://github.com/solomein-sv).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/static-files.md`. PR [#9580](https://github.com/tiangolo/fastapi/pull/9580) by [@Alexandrhub](https://github.com/Alexandrhub).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/query-params.md`. PR [#9584](https://github.com/tiangolo/fastapi/pull/9584) by [@Alexandrhub](https://github.com/Alexandrhub).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/first-steps.md`. PR [#9471](https://github.com/tiangolo/fastapi/pull/9471) by [@AGolicyn](https://github.com/AGolicyn).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/debugging.md`. PR [#9579](https://github.com/tiangolo/fastapi/pull/9579) by [@Alexandrhub](https://github.com/Alexandrhub).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/path-params.md`. PR [#9519](https://github.com/tiangolo/fastapi/pull/9519) by [@AGolicyn](https://github.com/AGolicyn).
+* 🌐 Add Chinese translation for `docs/zh/docs/tutorial/static-files.md`. PR [#9436](https://github.com/tiangolo/fastapi/pull/9436) by [@wdh99](https://github.com/wdh99).
+* 🌐 Update Spanish translation including new illustrations in `docs/es/docs/async.md`. PR [#9483](https://github.com/tiangolo/fastapi/pull/9483) by [@andresbermeoq](https://github.com/andresbermeoq).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/path-params-numeric-validations.md`. PR [#9563](https://github.com/tiangolo/fastapi/pull/9563) by [@ivan-abc](https://github.com/ivan-abc).
+* 🌐 Add Russian translation for `docs/ru/docs/deployment/concepts.md`. PR [#9577](https://github.com/tiangolo/fastapi/pull/9577) by [@Xewus](https://github.com/Xewus).
+* 🌐 Add Russian translation for `docs/ru/docs/tutorial/body-multiple-params.md`. PR [#9586](https://github.com/tiangolo/fastapi/pull/9586) by [@Alexandrhub](https://github.com/Alexandrhub).
+
+### Internal
+
+* 👥 Update FastAPI People. PR [#9602](https://github.com/tiangolo/fastapi/pull/9602) by [@github-actions[bot]](https://github.com/apps/github-actions).
+* 🔧 Update sponsors, remove InvestSuite. PR [#9612](https://github.com/tiangolo/fastapi/pull/9612) by [@tiangolo](https://github.com/tiangolo).
+
 ## 0.95.2
 
 * ⬆️ Upgrade Starlette version to `>=0.27.0` for a security release. PR [#9541](https://github.com/tiangolo/fastapi/pull/9541) by [@tiangolo](https://github.com/tiangolo). Details on [Starlette's security advisory](https://github.com/encode/starlette/security/advisories/GHSA-v5gw-mw7f-84px).
 
 ### Translations
 
 * 🌐 Add Portuguese translation for `docs/pt/docs/advanced/events.md`. PR [#9326](https://github.com/tiangolo/fastapi/pull/9326) by [@oandersonmagalhaes](https://github.com/oandersonmagalhaes).
```

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/additional-responses.md` & `fastapi-0.96.0/docs/en/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/en/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/advanced-dependencies.md` & `fastapi-0.96.0/docs/en/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/async-sql-databases.md` & `fastapi-0.96.0/docs/en/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/async-tests.md` & `fastapi-0.96.0/docs/en/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/behind-a-proxy.md` & `fastapi-0.96.0/docs/en/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/conditional-openapi.md` & `fastapi-0.96.0/docs/en/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/custom-request-and-route.md` & `fastapi-0.96.0/docs/en/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/custom-response.md` & `fastapi-0.96.0/docs/en/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/dataclasses.md` & `fastapi-0.96.0/docs/en/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/events.md` & `fastapi-0.96.0/docs/en/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/extending-openapi.md` & `fastapi-0.96.0/docs/en/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/generate-clients.md` & `fastapi-0.96.0/docs/en/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/graphql.md` & `fastapi-0.96.0/docs/en/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/index.md` & `fastapi-0.96.0/docs/en/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/middleware.md` & `fastapi-0.96.0/docs/en/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/nosql-databases.md` & `fastapi-0.96.0/docs/en/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/openapi-callbacks.md` & `fastapi-0.96.0/docs/en/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/en/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/response-change-status-code.md` & `fastapi-0.96.0/docs/en/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/response-cookies.md` & `fastapi-0.96.0/docs/en/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/en/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/response-headers.md` & `fastapi-0.96.0/docs/en/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/settings.md` & `fastapi-0.96.0/docs/en/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/sql-databases-peewee.md` & `fastapi-0.96.0/docs/en/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/sub-applications.md` & `fastapi-0.96.0/docs/en/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/templates.md` & `fastapi-0.96.0/docs/en/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/testing-database.md` & `fastapi-0.96.0/docs/en/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/testing-dependencies.md` & `fastapi-0.96.0/docs/en/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/using-request-directly.md` & `fastapi-0.96.0/docs/en/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/websockets.md` & `fastapi-0.96.0/docs/en/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/wsgi.md` & `fastapi-0.96.0/docs/en/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/security/http-basic-auth.md` & `fastapi-0.96.0/docs/en/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/security/index.md` & `fastapi-0.96.0/docs/en/docs/advanced/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.96.0/docs/en/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/css/custom.css` & `fastapi-0.96.0/docs/en/docs/css/custom.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/css/termynal.css` & `fastapi-0.96.0/docs/en/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/concepts.md` & `fastapi-0.96.0/docs/en/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/deta.md` & `fastapi-0.96.0/docs/en/docs/deployment/deta.md`

 * *Files identical despite different names*

```diff
@@ -272,15 +272,15 @@
 
 Congrats! You deployed your FastAPI app to Deta Space! 🎉 🍰
 
 Also, notice that Deta Space correctly handles HTTPS for you, so you don't have to take care of that and can be sure that your users will have a secure encrypted connection. ✅ 🔒
 
 ## Create a release
 
-Space also allows you to publish your API. When you publish it, anyone else can install their own copy of your API, in their own Data Space cloud.
+Space also allows you to publish your API. When you publish it, anyone else can install their own copy of your API, in their own Deta Space cloud.
 
 To do so, run `space release` in the Space CLI to create an **unlisted release**:
 
 <div class="termy">
 
 ```console
 $ space release
```

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/docker.md` & `fastapi-0.96.0/docs/en/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/https.md` & `fastapi-0.96.0/docs/en/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/index.md` & `fastapi-0.96.0/docs/en/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/manually.md` & `fastapi-0.96.0/docs/en/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/server-workers.md` & `fastapi-0.96.0/docs/en/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/deployment/versions.md` & `fastapi-0.96.0/docs/en/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/github-social-preview.png` & `fastapi-0.96.0/docs/en/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/github-social-preview.svg` & `fastapi-0.96.0/docs/en/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/icon-transparent-bg.png` & `fastapi-0.96.0/docs/en/docs/img/icon-transparent-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/icon-white-bg.png` & `fastapi-0.96.0/docs/en/docs/img/icon-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/icon-white.svg` & `fastapi-0.96.0/docs/en/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-teal-vector.svg` & `fastapi-0.96.0/docs/en/docs/img/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-teal.svg` & `fastapi-0.96.0/docs/en/docs/img/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/pycharm-completion.png` & `fastapi-0.96.0/docs/en/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/vscode-completion.png` & `fastapi-0.96.0/docs/en/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png` & `fastapi-0.96.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png` & `fastapi-0.96.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/concepts/image01.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/concepts/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/concepts/process-ram.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/concepts/process-ram.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/concepts/process-ram.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/concepts/process-ram.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image01.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image02.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image03.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image04.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image05.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/deta/image06.png` & `fastapi-0.96.0/docs/en/docs/img/deployment/deta/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https01.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https01.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https01.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https01.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https02.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https02.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https02.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https02.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https03.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https03.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https03.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https03.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https04.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https04.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https04.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https04.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https05.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https05.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https05.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https05.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https06.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https06.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https06.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https06.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https07.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https07.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https07.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https07.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https08.drawio` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https08.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/deployment/https/https08.svg` & `fastapi-0.96.0/docs/en/docs/img/deployment/https/https08.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-01-swagger-ui-simple.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-02-redoc-simple.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-02-redoc-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-03-swagger-02.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-03-swagger-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-04-swagger-03.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-04-swagger-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-05-swagger-04.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-05-swagger-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/index/index-06-redoc-02.png` & `fastapi-0.96.0/docs/en/docs/img/index/index-06-redoc-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal-vector.svg` & `fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal.png` & `fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-teal.svg` & `fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/logo-margin/logo-white-bg.png` & `fastapi-0.96.0/docs/en/docs/img/logo-margin/logo-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image01.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image02.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image03.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image04.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image05.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/python-types/image06.png` & `fastapi-0.96.0/docs/en/docs/img/python-types/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/budget-insight.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/budget-insight.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/calmcode.jpg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/calmcode.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/classiq-banner.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/classiq-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/classiq.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/classiq.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/cryptapi-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/cryptapi-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/cryptapi.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/cryptapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/databento.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/databento.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/deta-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/deta-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/deta.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/deta.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/docarray-top-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/docarray-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/docarray.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/docarray.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/doist-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/doist-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/doist.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/doist.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/dropbase-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/dropbase-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/dropbase.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/dropbase.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/exoflare.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/exoflare.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/haystack-fastapi.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/haystack-fastapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/imgwhale-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/imgwhale-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/imgwhale.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/imgwhale.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/ines-course.jpg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/ines-course.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/investsuite.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/investsuite.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina-ai-banner.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina-ai-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina-ai.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina-ai.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina-top-banner.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/jina2.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/jina2.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/powens.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/powens.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks-banner.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/striveworks2.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/striveworks2.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/svix.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/svix.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/talkpython.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/talkpython.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/testdriven.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/testdriven.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/vimso.png` & `fastapi-0.96.0/docs/en/docs/img/sponsors/vimso.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/sponsors/wetransfer.svg` & `fastapi-0.96.0/docs/en/docs/img/sponsors/wetransfer.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/additional-responses/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/additional-responses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/async-sql-databases/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/behind-a-proxy/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/package.drawio` & `fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/bigger-applications/package.svg` & `fastapi-0.96.0/docs/en/docs/img/tutorial/bigger-applications/package.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body/image05.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body-fields/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body-fields/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body-fields/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body-fields/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/body-nested-models/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/body-nested-models/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/custom-response/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/custom-response/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/dataclasses/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/dataclasses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/debugging/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/debugging/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/debugging/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/debugging/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/dependencies/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/dependencies/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/dependencies/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/dependencies/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/extending-openapi/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/extending-openapi/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image05.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image06.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image07.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/generate-clients/image08.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/generate-clients/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/graphql/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/graphql/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/metadata/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/metadata/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/metadata/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/metadata/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/openapi-callbacks/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-operation-configuration/image05.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/path-params/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/path-params/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/query-params-str-validations/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/query-params-str-validations/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/response-model/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/response-model/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/response-model/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/response-model/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/response-status-code/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/response-status-code/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/response-status-code/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/response-status-code/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image05.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image06.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image07.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image08.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image09.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image09.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image10.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image10.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image11.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image11.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/security/image12.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/security/image12.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/sql-databases/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/sql-databases/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/sql-databases/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/sub-applications/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/sub-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/sub-applications/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/sub-applications/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image01.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image02.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image03.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image04.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/img/tutorial/websockets/image05.png` & `fastapi-0.96.0/docs/en/docs/img/tutorial/websockets/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/js/custom.js` & `fastapi-0.96.0/docs/en/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/js/termynal.js` & `fastapi-0.96.0/docs/en/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/background-tasks.md` & `fastapi-0.96.0/docs/en/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/bigger-applications.md` & `fastapi-0.96.0/docs/en/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/body-fields.md` & `fastapi-0.96.0/docs/en/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/body-multiple-params.md` & `fastapi-0.96.0/docs/en/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/body-nested-models.md` & `fastapi-0.96.0/docs/en/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/body-updates.md` & `fastapi-0.96.0/docs/en/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/body.md` & `fastapi-0.96.0/docs/en/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/en/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/cors.md` & `fastapi-0.96.0/docs/en/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/debugging.md` & `fastapi-0.96.0/docs/en/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/encoder.md` & `fastapi-0.96.0/docs/en/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/extra-data-types.md` & `fastapi-0.96.0/docs/en/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/extra-models.md` & `fastapi-0.96.0/docs/en/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/en/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/handling-errors.md` & `fastapi-0.96.0/docs/en/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/en/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/index.md` & `fastapi-0.96.0/docs/en/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/metadata.md` & `fastapi-0.96.0/docs/en/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/middleware.md` & `fastapi-0.96.0/docs/en/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/path-operation-configuration.md` & `fastapi-0.96.0/docs/en/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.96.0/docs/en/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/en/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/en/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/en/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/request-files.md` & `fastapi-0.96.0/docs/en/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/request-forms-and-files.md` & `fastapi-0.96.0/docs/en/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/request-forms.md` & `fastapi-0.96.0/docs/en/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/response-model.md` & `fastapi-0.96.0/docs/en/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/en/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/schema-extra-example.md` & `fastapi-0.96.0/docs/en/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/sql-databases.md` & `fastapi-0.96.0/docs/en/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/static-files.md` & `fastapi-0.96.0/docs/en/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/testing.md` & `fastapi-0.96.0/docs/en/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/index.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.96.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/security/first-steps.md` & `fastapi-0.96.0/docs/en/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/security/get-current-user.md` & `fastapi-0.96.0/docs/en/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/security/index.md` & `fastapi-0.96.0/docs/en/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.96.0/docs/en/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.96.0/docs/en/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/en/overrides/main.html` & `fastapi-0.96.0/docs/en/overrides/main.html`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/mkdocs.yml` & `fastapi-0.96.0/docs/es/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/async.md` & `fastapi-0.96.0/docs/es/docs/async.md`

 * *Files 5% similar despite different names*

```diff
@@ -100,32 +100,48 @@
 
 Para entender las diferencias, imagina la siguiente historia sobre hamburguesas:
 
 ### Hamburguesas Concurrentes
 
 Vas con la persona que te gusta 😍 a pedir comida rápida 🍔, haces cola mientras el cajero 💁 recoge los pedidos de las personas de delante tuyo.
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-01.png" alt="illustration">
+
 Llega tu turno, haces tu pedido de 2 hamburguesas impresionantes para esa persona 😍 y para ti.
 
-Pagas 💸.
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-02.png" alt="illustration">
 
 El cajero 💁 le dice algo al chico de la cocina 👨‍🍳 para que sepa que tiene que preparar tus hamburguesas 🍔 (a pesar de que actualmente está preparando las de los clientes anteriores).
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-03.png" alt="illustration">
+
+Pagas 💸.
 El cajero 💁 te da el número de tu turno.
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-04.png" alt="illustration">
+
 Mientras esperas, vas con esa persona 😍 y eliges una mesa, se sientan y hablan durante un rato largo (ya que las hamburguesas son muy impresionantes y necesitan un rato para prepararse ✨🍔✨).
 
 Mientras te sientas en la mesa con esa persona 😍, esperando las hamburguesas 🍔, puedes disfrutar ese tiempo admirando lo increíble, inteligente, y bien que se ve ✨😍✨.
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-05.png" alt="illustration">
+
 Mientras esperas y hablas con esa persona 😍, de vez en cuando, verificas el número del mostrador para ver si ya es tu turno.
 
 Al final, en algún momento, llega tu turno. Vas al mostrador, coges tus hamburguesas 🍔 y vuelves a la mesa.
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-06.png" alt="illustration">
+
 Tú y esa persona 😍 se comen las hamburguesas 🍔 y la pasan genial ✨.
 
+<img src="https://fastapi.tiangolo.com/img/async/concurrent-burgers/concurrent-burgers-07.png" alt="illustration">
+
+!!! info
+     Las ilustraciones fueron creados por <a href="https://www.instagram.com/ketrinadrawsalot" class="external-link" target="_blank">Ketrina Thompson</a>. 🎨
+
 ---
 
 Imagina que eres el sistema / programa 🤖 en esa historia.
 
 Mientras estás en la cola, estás quieto 😴, esperando tu turno, sin hacer nada muy "productivo". Pero la línea va rápida porque el cajero 💁 solo recibe los pedidos (no los prepara), así que está bien.
 
 Luego, cuando llega tu turno, haces un trabajo "productivo" real 🤓, procesas el menú, decides lo que quieres, lo que quiere esa persona 😍, pagas 💸, verificas que das el billete o tarjeta correctos, verificas que te cobren correctamente, que el pedido tiene los artículos correctos, etc.
@@ -146,34 +162,49 @@
 
 Vas con la persona que te gusta 😍 por comida rápida paralela 🍔.
 
 Haces la cola mientras varios cajeros (digamos 8) que a la vez son cocineros 👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳 toman los pedidos de las personas que están delante de ti.
 
 Todos los que están antes de ti están esperando 🕙 que sus hamburguesas 🍔 estén listas antes de dejar el mostrador porque cada uno de los 8 cajeros prepara la hamburguesa de inmediato antes de recibir el siguiente pedido.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-01.png" alt="illustration">
+
 Entonces finalmente es tu turno, haces tu pedido de 2 hamburguesas 🍔 impresionantes para esa persona 😍 y para ti.
 
 Pagas 💸.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-02.png" alt="illustration">
+
 El cajero va a la cocina 👨‍🍳.
 
 Esperas, de pie frente al mostrador 🕙, para que nadie más recoja tus hamburguesas 🍔, ya que no hay números para los turnos.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-03.png" alt="illustration">
+
 Como tu y esa persona 😍 están ocupados en impedir que alguien se ponga delante y recoja tus hamburguesas apenas llegan 🕙, tampoco puedes prestarle atención a esa persona 😞.
 
 Este es un trabajo "síncrono", estás "sincronizado" con el cajero / cocinero 👨‍🍳. Tienes que esperar y estar allí en el momento exacto en que el cajero / cocinero 👨‍🍳 termina las hamburguesas 🍔 y te las da, o de lo contrario, alguien más podría cogerlas.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-04.png" alt="illustration">
+
 Luego, el cajero / cocinero 👨‍🍳 finalmente regresa con tus hamburguesas 🍔, después de mucho tiempo esperando 🕙 frente al mostrador.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-05.png" alt="illustration">
+
 Cojes tus hamburguesas 🍔 y vas a la mesa con esa persona 😍.
 
 Sólo las comes y listo 🍔 ⏹.
 
+<img src="https://fastapi.tiangolo.com/img/async/parallel-burgers/parallel-burgers-06.png" alt="illustration">
+
 No has hablado ni coqueteado mucho, ya que has pasado la mayor parte del tiempo esperando 🕙 frente al mostrador 😞.
 
+!!! info
+     Las ilustraciones fueron creados por <a href="https://www.instagram.com/ketrinadrawsalot" class="external-link" target="_blank">Ketrina Thompson</a>. 🎨
+
 ---
 
 En este escenario de las hamburguesas paralelas, tú eres un sistema / programa 🤖 con dos procesadores (tú y la persona que te gusta 😍), ambos esperando 🕙 y dedicando su atención ⏯ a estar "esperando en el mostrador" 🕙 durante mucho tiempo.
 
 La tienda de comida rápida tiene 8 procesadores (cajeros / cocineros) 👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳. Mientras que la tienda de hamburguesas concurrentes podría haber tenido solo 2 (un cajero y un cocinero) 💁 👨‍🍳.
 
 Pero aún así, la experiencia final no es la mejor 😞.
@@ -236,15 +267,15 @@
 
 Tomaría la misma cantidad de tiempo terminar con o sin turnos (concurrencia) y habrías hecho la misma cantidad de trabajo.
 
 Pero en este caso, si pudieras traer a los 8 ex cajeros / cocineros / ahora limpiadores 👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳👨‍🍳, y cada uno de ellos (y tú) podría tomar una zona de la casa para limpiarla, podría hacer todo el trabajo en **paralelo**, con la ayuda adicional y terminar mucho antes.
 
 En este escenario, cada uno de los limpiadores (incluido tú) sería un procesador, haciendo su parte del trabajo.
 
-Y como la mayor parte del tiempo de ejecución lo coge el trabajo real (en lugar de esperar), y el trabajo en un sistema lo realiza una <abbr title = "Central Processing Unit. En español: Unidad Central de Procesamiento."> CPU </abbr>, a estos problemas se les llama "<abbr title="En español: atado a CPU.">CPU bond</abbr>".
+Y como la mayor parte del tiempo de ejecución lo coge el trabajo real (en lugar de esperar), y el trabajo en un sistema lo realiza una <abbr title = "Central Processing Unit. En español: Unidad Central de Procesamiento."> CPU </abbr>, a estos problemas se les llama "<abbr title="En español: atado a CPU.">CPU bound</abbr>".
 
 ---
 
 Ejemplos típicos de operaciones dependientes de CPU son cosas que requieren un procesamiento matemático complejo.
 
 Por ejemplo:
 
@@ -253,15 +284,15 @@
 * **Machine Learning**: normalmente requiere muchas multiplicaciones de "matrices" y "vectores". Imagina en una enorme hoja de cálculo con números y tener que multiplicarlos todos al mismo tiempo.
 * **Deep Learning**: este es un subcampo de Machine Learning, por lo tanto, aplica lo mismo. Es solo que no hay una sola hoja de cálculo de números para multiplicar, sino un gran conjunto de ellas, y en muchos casos, usa un procesador especial para construir y / o usar esos modelos.
 
 ### Concurrencia + Paralelismo: Web + Machine Learning
 
 Con **FastAPI** puedes aprovechar la concurrencia que es muy común para el desarrollo web (atractivo principal de NodeJS).
 
-Pero también puedes aprovechar los beneficios del paralelismo y el multiprocesamiento (tener múltiples procesos ejecutándose en paralelo) para cargas de trabajo **CPU bond** como las de los sistemas de Machine Learning.
+Pero también puedes aprovechar los beneficios del paralelismo y el multiprocesamiento (tener múltiples procesos ejecutándose en paralelo) para cargas de trabajo **CPU bound** como las de los sistemas de Machine Learning.
 
 Eso, más el simple hecho de que Python es el lenguaje principal para **Data Science**, Machine Learning y especialmente Deep Learning, hacen de FastAPI una muy buena combinación para las API y aplicaciones web de Data Science / Machine Learning (entre muchas otras).
 
 Para ver cómo lograr este paralelismo en producción, consulta la sección sobre [Despliegue](deployment/index.md){.internal-link target=_blank}.
 
 ## `async` y `await`
```

### Comparing `fastapi-0.95.2/docs/es/docs/features.md` & `fastapi-0.96.0/docs/es/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/index.md` & `fastapi-0.96.0/docs/es/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/python-types.md` & `fastapi-0.96.0/docs/es/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/es/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/advanced/index.md` & `fastapi-0.96.0/docs/es/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/es/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/es/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/es/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/tutorial/index.md` & `fastapi-0.96.0/docs/es/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/es/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/es/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/es/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fa/mkdocs.yml` & `fastapi-0.96.0/docs/fa/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fa/docs/index.md` & `fastapi-0.96.0/docs/fa/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/mkdocs.yml` & `fastapi-0.96.0/docs/fr/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/alternatives.md` & `fastapi-0.96.0/docs/fr/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/async.md` & `fastapi-0.96.0/docs/fr/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/external-links.md` & `fastapi-0.96.0/docs/fr/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/fastapi-people.md` & `fastapi-0.96.0/docs/fr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/features.md` & `fastapi-0.96.0/docs/fr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/help-fastapi.md` & `fastapi-0.96.0/docs/fr/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/history-design-future.md` & `fastapi-0.96.0/docs/fr/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/index.md` & `fastapi-0.96.0/docs/fr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/project-generation.md` & `fastapi-0.96.0/docs/fr/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/python-types.md` & `fastapi-0.96.0/docs/fr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/advanced/additional-responses.md` & `fastapi-0.96.0/docs/fr/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/fr/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/advanced/index.md` & `fastapi-0.96.0/docs/fr/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/fr/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/deta.md` & `fastapi-0.96.0/docs/fr/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/docker.md` & `fastapi-0.96.0/docs/fr/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/https.md` & `fastapi-0.96.0/docs/fr/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/index.md` & `fastapi-0.96.0/docs/fr/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/manually.md` & `fastapi-0.96.0/docs/fr/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/deployment/versions.md` & `fastapi-0.96.0/docs/fr/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/background-tasks.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/body.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/debugging.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/fr/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/fr/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/he/mkdocs.yml` & `fastapi-0.96.0/docs/he/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/he/docs/index.md` & `fastapi-0.96.0/docs/he/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/hy/mkdocs.yml` & `fastapi-0.96.0/docs/hy/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/hy/docs/index.md` & `fastapi-0.96.0/docs/hy/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/id/mkdocs.yml` & `fastapi-0.96.0/docs/id/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/id/docs/index.md` & `fastapi-0.96.0/docs/id/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/id/docs/tutorial/index.md` & `fastapi-0.96.0/docs/id/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/it/mkdocs.yml` & `fastapi-0.96.0/docs/it/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/it/docs/index.md` & `fastapi-0.96.0/docs/it/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/mkdocs.yml` & `fastapi-0.96.0/docs/ja/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/alternatives.md` & `fastapi-0.96.0/docs/ja/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/async.md` & `fastapi-0.96.0/docs/ja/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/benchmarks.md` & `fastapi-0.96.0/docs/ja/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/contributing.md` & `fastapi-0.96.0/docs/ja/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/external-links.md` & `fastapi-0.96.0/docs/ja/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/fastapi-people.md` & `fastapi-0.96.0/docs/ja/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/features.md` & `fastapi-0.96.0/docs/ja/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/help-fastapi.md` & `fastapi-0.96.0/docs/ja/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/history-design-future.md` & `fastapi-0.96.0/docs/ja/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/index.md` & `fastapi-0.96.0/docs/ja/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/project-generation.md` & `fastapi-0.96.0/docs/ja/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/ja/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/conditional-openapi.md` & `fastapi-0.96.0/docs/ja/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/custom-response.md` & `fastapi-0.96.0/docs/ja/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/index.md` & `fastapi-0.96.0/docs/ja/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/nosql-databases.md` & `fastapi-0.96.0/docs/ja/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/ja/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/advanced/websockets.md` & `fastapi-0.96.0/docs/ja/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/deployment/deta.md` & `fastapi-0.96.0/docs/ja/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/deployment/docker.md` & `fastapi-0.96.0/docs/ja/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/deployment/manually.md` & `fastapi-0.96.0/docs/ja/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/deployment/versions.md` & `fastapi-0.96.0/docs/ja/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/body-updates.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/body.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/cors.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/debugging.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/index.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/middleware.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/request-forms.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/static-files.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/testing.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/security/first-steps.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ja/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.96.0/docs/ja/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/mkdocs.yml` & `fastapi-0.96.0/docs/ko/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/index.md` & `fastapi-0.96.0/docs/ko/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/deployment/versions.md` & `fastapi-0.96.0/docs/ko/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/cors.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/encoder.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/index.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/request-files.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/request-forms-and-files.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.96.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/lo/mkdocs.yml` & `fastapi-0.96.0/docs/lo/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/lo/docs/index.md` & `fastapi-0.96.0/docs/lo/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/nl/mkdocs.yml` & `fastapi-0.96.0/docs/nl/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/nl/docs/index.md` & `fastapi-0.96.0/docs/nl/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pl/mkdocs.yml` & `fastapi-0.96.0/docs/pl/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pl/docs/index.md` & `fastapi-0.96.0/docs/pl/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pl/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/pl/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pl/docs/tutorial/index.md` & `fastapi-0.96.0/docs/pl/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/mkdocs.yml` & `fastapi-0.96.0/docs/pt/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/alternatives.md` & `fastapi-0.96.0/docs/pt/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/async.md` & `fastapi-0.96.0/docs/pt/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/benchmarks.md` & `fastapi-0.96.0/docs/pt/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/contributing.md` & `fastapi-0.96.0/docs/pt/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/deployment.md` & `fastapi-0.96.0/docs/pt/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/external-links.md` & `fastapi-0.96.0/docs/pt/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/fastapi-people.md` & `fastapi-0.96.0/docs/pt/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/features.md` & `fastapi-0.96.0/docs/pt/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/help-fastapi.md` & `fastapi-0.96.0/docs/pt/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/history-design-future.md` & `fastapi-0.96.0/docs/pt/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/index.md` & `fastapi-0.96.0/docs/pt/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/project-generation.md` & `fastapi-0.96.0/docs/pt/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/python-types.md` & `fastapi-0.96.0/docs/pt/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/advanced/events.md` & `fastapi-0.96.0/docs/pt/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/advanced/index.md` & `fastapi-0.96.0/docs/pt/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/deployment/deta.md` & `fastapi-0.96.0/docs/pt/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/deployment/docker.md` & `fastapi-0.96.0/docs/pt/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/deployment/https.md` & `fastapi-0.96.0/docs/pt/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/deployment/versions.md` & `fastapi-0.96.0/docs/pt/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/background-tasks.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/body-fields.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/body-multiple-params.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/body-nested-models.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/body.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/encoder.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/extra-data-types.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/extra-models.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/handling-errors.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/index.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/path-operation-configuration.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/request-forms-and-files.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/request-forms.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/static-files.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/security/first-steps.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/pt/docs/tutorial/security/index.md` & `fastapi-0.96.0/docs/pt/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/mkdocs.yml` & `fastapi-0.96.0/docs/ru/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -63,25 +63,33 @@
   - tr: /tr/
   - uk: /uk/
   - zh: /zh/
 - features.md
 - fastapi-people.md
 - python-types.md
 - Учебник - руководство пользователя:
+  - tutorial/first-steps.md
+  - tutorial/path-params.md
   - tutorial/query-params-str-validations.md
+  - tutorial/path-params-numeric-validations.md
   - tutorial/body-fields.md
   - tutorial/background-tasks.md
   - tutorial/extra-data-types.md
   - tutorial/cookie-params.md
   - tutorial/testing.md
   - tutorial/response-status-code.md
+  - tutorial/query-params.md
+  - tutorial/body-multiple-params.md
+  - tutorial/static-files.md
+  - tutorial/debugging.md
 - async.md
 - Развёртывание:
   - deployment/index.md
   - deployment/versions.md
+  - deployment/concepts.md
   - deployment/https.md
   - deployment/manually.md
 - project-generation.md
 - alternatives.md
 - history-design-future.md
 - external-links.md
 - benchmarks.md
```

### Comparing `fastapi-0.95.2/docs/ru/docs/alternatives.md` & `fastapi-0.96.0/docs/ru/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/async.md` & `fastapi-0.96.0/docs/ru/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/benchmarks.md` & `fastapi-0.96.0/docs/ru/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/contributing.md` & `fastapi-0.96.0/docs/ru/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/external-links.md` & `fastapi-0.96.0/docs/ru/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/fastapi-people.md` & `fastapi-0.96.0/docs/ru/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/features.md` & `fastapi-0.96.0/docs/ru/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/help-fastapi.md` & `fastapi-0.96.0/docs/ru/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/history-design-future.md` & `fastapi-0.96.0/docs/ru/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/index.md` & `fastapi-0.96.0/docs/ru/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/project-generation.md` & `fastapi-0.96.0/docs/ru/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/python-types.md` & `fastapi-0.96.0/docs/ru/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/deployment/https.md` & `fastapi-0.96.0/docs/ru/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/deployment/index.md` & `fastapi-0.96.0/docs/ru/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/deployment/manually.md` & `fastapi-0.96.0/docs/ru/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/deployment/versions.md` & `fastapi-0.96.0/docs/ru/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/background-tasks.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/body-fields.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/extra-data-types.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ru/docs/tutorial/testing.md` & `fastapi-0.96.0/docs/ru/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/sq/mkdocs.yml` & `fastapi-0.96.0/docs/sq/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/sq/docs/index.md` & `fastapi-0.96.0/docs/sq/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/sv/mkdocs.yml` & `fastapi-0.96.0/docs/sv/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/sv/docs/index.md` & `fastapi-0.96.0/docs/sv/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/ta/mkdocs.yml` & `fastapi-0.96.0/docs/ta/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/mkdocs.yml` & `fastapi-0.96.0/docs/tr/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/benchmarks.md` & `fastapi-0.96.0/docs/tr/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/fastapi-people.md` & `fastapi-0.96.0/docs/tr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/features.md` & `fastapi-0.96.0/docs/tr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/index.md` & `fastapi-0.96.0/docs/tr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/python-types.md` & `fastapi-0.96.0/docs/tr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/tr/docs/tutorial/first_steps.md` & `fastapi-0.96.0/docs/tr/docs/tutorial/first_steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/uk/mkdocs.yml` & `fastapi-0.96.0/docs/uk/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/uk/docs/index.md` & `fastapi-0.96.0/docs/uk/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/mkdocs.yml` & `fastapi-0.96.0/docs/zh/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     - tutorial/security/get-current-user.md
     - tutorial/security/simple-oauth2.md
     - tutorial/security/oauth2-jwt.md
   - tutorial/cors.md
   - tutorial/sql-databases.md
   - tutorial/bigger-applications.md
   - tutorial/metadata.md
+  - tutorial/static-files.md
   - tutorial/debugging.md
 - 高级用户指南:
   - advanced/index.md
   - advanced/path-operation-advanced-configuration.md
   - advanced/additional-status-codes.md
   - advanced/response-directly.md
   - advanced/custom-response.md
```

### Comparing `fastapi-0.95.2/docs/zh/docs/benchmarks.md` & `fastapi-0.96.0/docs/zh/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/contributing.md` & `fastapi-0.96.0/docs/zh/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/fastapi-people.md` & `fastapi-0.96.0/docs/zh/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/features.md` & `fastapi-0.96.0/docs/zh/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/help-fastapi.md` & `fastapi-0.96.0/docs/zh/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/index.md` & `fastapi-0.96.0/docs/zh/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/python-types.md` & `fastapi-0.96.0/docs/zh/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/additional-status-codes.md` & `fastapi-0.96.0/docs/zh/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/custom-response.md` & `fastapi-0.96.0/docs/zh/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/index.md` & `fastapi-0.96.0/docs/zh/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.96.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/response-cookies.md` & `fastapi-0.96.0/docs/zh/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/response-directly.md` & `fastapi-0.96.0/docs/zh/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/advanced/wsgi.md` & `fastapi-0.96.0/docs/zh/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/bigger-applications.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/body-fields.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/body-multiple-params.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/body-nested-models.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/body-updates.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/body.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/cookie-params.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/cors.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/debugging.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/encoder.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/extra-data-types.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/extra-models.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/first-steps.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/handling-errors.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/header-params.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/index.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/metadata.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/middleware.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/path-operation-configuration.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/path-params.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/query-params-str-validations.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/query-params.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/request-files.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/request-forms-and-files.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/request-forms.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/response-model.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/response-status-code.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/schema-extra-example.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/sql-databases.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/index.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/security/first-steps.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/security/get-current-user.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/security/index.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs/zh/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.96.0/docs/zh/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_responses/tutorial002.py` & `fastapi-0.96.0/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_responses/tutorial003.py` & `fastapi-0.96.0/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_responses/tutorial004.py` & `fastapi-0.96.0/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_status_codes/tutorial001.py` & `fastapi-0.96.0/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an.py` & `fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an_py310.py` & `fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_an_py39.py` & `fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/additional_status_codes/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/tutorial002.py` & `fastapi-0.96.0/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/tutorial003.py` & `fastapi-0.96.0/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b/main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b/test_main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an/main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an/test_main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an_py310/main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an_py310/test_main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an_py39/main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_an_py39/test_main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_py310/main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/app_testing/app_b_py310/test_main.py` & `fastapi-0.96.0/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/async_sql_databases/tutorial001.py` & `fastapi-0.96.0/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial001.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial002.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial002_an.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial002_an_py310.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial002_an_py39.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/background_tasks/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app/main.py` & `fastapi-0.96.0/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app/routers/items.py` & `fastapi-0.96.0/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app_an/main.py` & `fastapi-0.96.0/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app_an/routers/items.py` & `fastapi-0.96.0/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/main.py` & `fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/bigger_applications/app_an_py39/routers/items.py` & `fastapi-0.96.0/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_fields/tutorial001.py` & `fastapi-0.96.0/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_fields/tutorial001_an.py` & `fastapi-0.96.0/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_fields/tutorial001_an_py310.py` & `fastapi-0.96.0/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_fields/tutorial001_an_py39.py` & `fastapi-0.96.0/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_fields/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial001.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an_py310.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_an_py39.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial003.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an_py310.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial003_an_py39.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial004.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an_py310.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_an_py39.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_multiple_params/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial005.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial005_py39.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial006.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial006_py39.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial007.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial007_py310.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_nested_models/tutorial007_py39.py` & `fastapi-0.96.0/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial001.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial001_py39.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial002.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/body_updates/tutorial002_py39.py` & `fastapi-0.96.0/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/custom_request_and_route/tutorial001.py` & `fastapi-0.96.0/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/custom_request_and_route/tutorial002.py` & `fastapi-0.96.0/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/custom_request_and_route/tutorial003.py` & `fastapi-0.96.0/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dataclasses/tutorial002.py` & `fastapi-0.96.0/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dataclasses/tutorial003.py` & `fastapi-0.96.0/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial002.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial002_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial002_an_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial002_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial003.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial003_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial003_an_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial003_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial003_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial004.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial004_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial004_an_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial004_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial005_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial005_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial006.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial006_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial006_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial008_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial008_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial011_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial011_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial012.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial012_an.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependencies/tutorial012_an_py39.py` & `fastapi-0.96.0/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependency_testing/tutorial001.py` & `fastapi-0.96.0/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an.py` & `fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an_py310.py` & `fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependency_testing/tutorial001_an_py39.py` & `fastapi-0.96.0/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/dependency_testing/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/events/tutorial003.py` & `fastapi-0.96.0/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extending_openapi/tutorial001.py` & `fastapi-0.96.0/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extending_openapi/tutorial002.py` & `fastapi-0.96.0/docs_src/extending_openapi/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_data_types/tutorial001.py` & `fastapi-0.96.0/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an.py` & `fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an_py310.py` & `fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_data_types/tutorial001_an_py39.py` & `fastapi-0.96.0/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_data_types/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial001.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial002.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial003.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/extra_models/tutorial003_py310.py` & `fastapi-0.96.0/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/generate_clients/tutorial001.py` & `fastapi-0.96.0/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/generate_clients/tutorial002.py` & `fastapi-0.96.0/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/generate_clients/tutorial002_py39.py` & `fastapi-0.96.0/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/generate_clients/tutorial003.py` & `fastapi-0.96.0/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/generate_clients/tutorial003_py39.py` & `fastapi-0.96.0/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/handling_errors/tutorial003.py` & `fastapi-0.96.0/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/handling_errors/tutorial004.py` & `fastapi-0.96.0/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/handling_errors/tutorial005.py` & `fastapi-0.96.0/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/handling_errors/tutorial006.py` & `fastapi-0.96.0/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/metadata/tutorial001.py` & `fastapi-0.96.0/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/metadata/tutorial004.py` & `fastapi-0.96.0/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/nosql_databases/tutorial001.py` & `fastapi-0.96.0/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/openapi_callbacks/tutorial001.py` & `fastapi-0.96.0/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial002.py` & `fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial004.py` & `fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial006.py` & `fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_advanced_configuration/tutorial007.py` & `fastapi-0.96.0/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial002_py39.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial003.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial003_py39.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial004_py39.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005_py310.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_operation_configuration/tutorial005_py39.py` & `fastapi-0.96.0/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/path_params/tutorial005.py` & `fastapi-0.96.0/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial008_an.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/query_params_str_validations/tutorial010_py310.py` & `fastapi-0.96.0/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial001_02_an.py` & `fastapi-0.96.0/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial001_02_an_py39.py` & `fastapi-0.96.0/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial002.py` & `fastapi-0.96.0/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial002_an.py` & `fastapi-0.96.0/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial002_an_py39.py` & `fastapi-0.96.0/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial002_py39.py` & `fastapi-0.96.0/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial003.py` & `fastapi-0.96.0/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial003_an.py` & `fastapi-0.96.0/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial003_an_py39.py` & `fastapi-0.96.0/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/request_files/tutorial003_py39.py` & `fastapi-0.96.0/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial001.py` & `fastapi-0.96.0/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial001_01.py` & `fastapi-0.96.0/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial001_py39.py` & `fastapi-0.96.0/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial004.py` & `fastapi-0.96.0/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial004_py39.py` & `fastapi-0.96.0/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial005.py` & `fastapi-0.96.0/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial005_py310.py` & `fastapi-0.96.0/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial006.py` & `fastapi-0.96.0/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/response_model/tutorial006_py310.py` & `fastapi-0.96.0/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial001.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial001_py310.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial003.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an_py310.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_an_py39.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial003_py310.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial004.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an_py310.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_an_py39.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/schema_extra_example/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/schema_extra_example/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial002.py` & `fastapi-0.96.0/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial002_an.py` & `fastapi-0.96.0/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial002_an_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial002_an_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial003.py` & `fastapi-0.96.0/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial003_an.py` & `fastapi-0.96.0/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial003_an_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial003_an_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial003_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial004.py` & `fastapi-0.96.0/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial004_an.py` & `fastapi-0.96.0/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial004_an_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial004_an_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial004_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005.py` & `fastapi-0.96.0/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005_an.py` & `fastapi-0.96.0/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005_an_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005_an_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005_py310.py` & `fastapi-0.96.0/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial005_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial007.py` & `fastapi-0.96.0/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial007_an.py` & `fastapi-0.96.0/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/security/tutorial007_an_py39.py` & `fastapi-0.96.0/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/settings/app02/test_main.py` & `fastapi-0.96.0/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/settings/app02_an/test_main.py` & `fastapi-0.96.0/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/settings/app02_an_py39/test_main.py` & `fastapi-0.96.0/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app/alt_main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app/crud.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app/main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app/models.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/alt_main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/crud.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/models.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/alt_main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/crud.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/main.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/models.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `fastapi-0.96.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/crud.py` & `fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/database.py` & `fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/main.py` & `fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/sql_databases_peewee/sql_app/schemas.py` & `fastapi-0.96.0/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial001.py` & `fastapi-0.96.0/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial002.py` & `fastapi-0.96.0/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial002_an.py` & `fastapi-0.96.0/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial002_an_py310.py` & `fastapi-0.96.0/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial002_an_py39.py` & `fastapi-0.96.0/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial002_py310.py` & `fastapi-0.96.0/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial003.py` & `fastapi-0.96.0/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/docs_src/websockets/tutorial003_py39.py` & `fastapi-0.96.0/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/__init__.py` & `fastapi-0.96.0/fastapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """FastAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.95.2"
+__version__ = "0.96.0"
 
 from starlette import status as status
 
 from .applications import FastAPI as FastAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `fastapi-0.95.2/fastapi/applications.py` & `fastapi-0.96.0/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/concurrency.py` & `fastapi-0.96.0/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/datastructures.py` & `fastapi-0.96.0/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/encoders.py` & `fastapi-0.96.0/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/exception_handlers.py` & `fastapi-0.96.0/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/exceptions.py` & `fastapi-0.96.0/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/param_functions.py` & `fastapi-0.96.0/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/params.py` & `fastapi-0.96.0/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/responses.py` & `fastapi-0.96.0/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/routing.py` & `fastapi-0.96.0/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/utils.py` & `fastapi-0.96.0/fastapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import re
 import warnings
 from dataclasses import is_dataclass
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Dict, Optional, Set, Type, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    MutableMapping,
+    Optional,
+    Set,
+    Type,
+    Union,
+    cast,
+)
+from weakref import WeakKeyDictionary
 
 import fastapi
 from fastapi.datastructures import DefaultPlaceholder, DefaultType
 from fastapi.openapi.constants import REF_PREFIX
 from pydantic import BaseConfig, BaseModel, create_model
 from pydantic.class_validators import Validator
 from pydantic.fields import FieldInfo, ModelField, UndefinedType
 from pydantic.schema import model_process_schema
 from pydantic.utils import lenient_issubclass
 
 if TYPE_CHECKING:  # pragma: nocover
     from .routing import APIRoute
 
+# Cache for `create_cloned_field`
+_CLONED_TYPES_CACHE: MutableMapping[
+    Type[BaseModel], Type[BaseModel]
+] = WeakKeyDictionary()
+
 
 def is_body_allowed_for_status_code(status_code: Union[int, str, None]) -> bool:
     if status_code is None:
         return True
     # Ref: https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#patterned-fields-1
     if status_code in {
         "default",
@@ -94,19 +110,21 @@
             "https://fastapi.tiangolo.com/tutorial/response-model/"
         ) from None
 
 
 def create_cloned_field(
     field: ModelField,
     *,
-    cloned_types: Optional[Dict[Type[BaseModel], Type[BaseModel]]] = None,
+    cloned_types: Optional[MutableMapping[Type[BaseModel], Type[BaseModel]]] = None,
 ) -> ModelField:
-    # _cloned_types has already cloned types, to support recursive models
+    # cloned_types caches already cloned types to support recursive models and improve
+    # performance by avoiding unecessary cloning
     if cloned_types is None:
-        cloned_types = {}
+        cloned_types = _CLONED_TYPES_CACHE
+
     original_type = field.type_
     if is_dataclass(original_type) and hasattr(original_type, "__pydantic_model__"):
         original_type = original_type.__pydantic_model__
     use_type = original_type
     if lenient_issubclass(original_type, BaseModel):
         original_type = cast(Type[BaseModel], original_type)
         use_type = cloned_types.get(original_type)
```

### Comparing `fastapi-0.95.2/fastapi/dependencies/models.py` & `fastapi-0.96.0/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/dependencies/utils.py` & `fastapi-0.96.0/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/middleware/asyncexitstack.py` & `fastapi-0.96.0/fastapi/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/openapi/docs.py` & `fastapi-0.96.0/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/openapi/models.py` & `fastapi-0.96.0/fastapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/openapi/utils.py` & `fastapi-0.96.0/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/security/__init__.py` & `fastapi-0.96.0/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/security/api_key.py` & `fastapi-0.96.0/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/security/http.py` & `fastapi-0.96.0/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/security/oauth2.py` & `fastapi-0.96.0/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/fastapi/security/open_id_connect_url.py` & `fastapi-0.96.0/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/scripts/docs.py` & `fastapi-0.96.0/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/scripts/gitter_releases_bot.py` & `fastapi-0.96.0/scripts/gitter_releases_bot.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/main.py` & `fastapi-0.96.0/tests/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_properties.py` & `fastapi-0.96.0/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_response_extra.py` & `fastapi-0.96.0/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_bad.py` & `fastapi-0.96.0/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_custom_model_in_callback.py` & `fastapi-0.96.0/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_custom_validationerror.py` & `fastapi-0.96.0/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_default_validationerror.py` & `fastapi-0.96.0/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_response_class.py` & `fastapi-0.96.0/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_additional_responses_router.py` & `fastapi-0.96.0/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_ambiguous_params.py` & `fastapi-0.96.0/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_annotated.py` & `fastapi-0.96.0/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_application.py` & `fastapi-0.96.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_custom_middleware_exception.py` & `fastapi-0.96.0/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_custom_route_class.py` & `fastapi-0.96.0/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_custom_schema_fields.py` & `fastapi-0.96.0/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_custom_swagger_ui_redirect.py` & `fastapi-0.96.0/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_datastructures.py` & `fastapi-0.96.0/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_datetime_custom_encoder.py` & `fastapi-0.96.0/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_default_response_class.py` & `fastapi-0.96.0/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_default_response_class_router.py` & `fastapi-0.96.0/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_cache.py` & `fastapi-0.96.0/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_class.py` & `fastapi-0.96.0/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_contextmanager.py` & `fastapi-0.96.0/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_contextvars.py` & `fastapi-0.96.0/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_duplicates.py` & `fastapi-0.96.0/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_normal_exceptions.py` & `fastapi-0.96.0/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_overrides.py` & `fastapi-0.96.0/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_dependency_security_overrides.py` & `fastapi-0.96.0/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_deprecated_openapi_prefix.py` & `fastapi-0.96.0/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_duplicate_models_openapi.py` & `fastapi-0.96.0/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_empty_router.py` & `fastapi-0.96.0/tests/test_empty_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_enforce_once_required_parameter.py` & `fastapi-0.96.0/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_exception_handlers.py` & `fastapi-0.96.0/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_extra_routes.py` & `fastapi-0.96.0/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_filter_pydantic_sub_model.py` & `fastapi-0.96.0/tests/test_filter_pydantic_sub_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_forms_from_non_typing_sequences.py` & `fastapi-0.96.0/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_generate_unique_id_function.py` & `fastapi-0.96.0/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_get_request_body.py` & `fastapi-0.96.0/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_http_connection_injection.py` & `fastapi-0.96.0/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_include_router_defaults_overrides.py` & `fastapi-0.96.0/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_infer_param_optionality.py` & `fastapi-0.96.0/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_inherited_custom_class.py` & `fastapi-0.96.0/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_invalid_path_param.py` & `fastapi-0.96.0/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_invalid_sequence_param.py` & `fastapi-0.96.0/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_jsonable_encoder.py` & `fastapi-0.96.0/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_local_docs.py` & `fastapi-0.96.0/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_multi_body_errors.py` & `fastapi-0.96.0/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_multi_query_errors.py` & `fastapi-0.96.0/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_multipart_installation.py` & `fastapi-0.96.0/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_no_swagger_ui_redirect.py` & `fastapi-0.96.0/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_openapi_query_parameter_extension.py` & `fastapi-0.96.0/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_openapi_route_extensions.py` & `fastapi-0.96.0/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_openapi_servers.py` & `fastapi-0.96.0/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_operations_signatures.py` & `fastapi-0.96.0/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_orjson_response_class.py` & `fastapi-0.96.0/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_param_class.py` & `fastapi-0.96.0/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_param_in_path_and_dependency.py` & `fastapi-0.96.0/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_param_include_in_schema.py` & `fastapi-0.96.0/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_params_repr.py` & `fastapi-0.96.0/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_path.py` & `fastapi-0.96.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_put_no_body.py` & `fastapi-0.96.0/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_query.py` & `fastapi-0.96.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_read_with_orm_mode.py` & `fastapi-0.96.0/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_repeated_cookie_headers.py` & `fastapi-0.96.0/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_repeated_dependency_schema.py` & `fastapi-0.96.0/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_repeated_parameter_alias.py` & `fastapi-0.96.0/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_reponse_set_reponse_code_empty.py` & `fastapi-0.96.0/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_request_body_parameters_media_type.py` & `fastapi-0.96.0/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_required_noneable.py` & `fastapi-0.96.0/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_by_alias.py` & `fastapi-0.96.0/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_change_status_code.py` & `fastapi-0.96.0/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_class_no_mediatype.py` & `fastapi-0.96.0/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_code_no_body.py` & `fastapi-0.96.0/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_model_as_return_annotation.py` & `fastapi-0.96.0/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_model_include_exclude.py` & `fastapi-0.96.0/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_model_invalid.py` & `fastapi-0.96.0/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_response_model_sub_types.py` & `fastapi-0.96.0/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_route_scope.py` & `fastapi-0.96.0/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_router_events.py` & `fastapi-0.96.0/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_schema_extra_examples.py` & `fastapi-0.96.0/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_cookie.py` & `fastapi-0.96.0/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_cookie_description.py` & `fastapi-0.96.0/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_cookie_optional.py` & `fastapi-0.96.0/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_header.py` & `fastapi-0.96.0/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_header_description.py` & `fastapi-0.96.0/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_header_optional.py` & `fastapi-0.96.0/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_query.py` & `fastapi-0.96.0/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_query_description.py` & `fastapi-0.96.0/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_api_key_query_optional.py` & `fastapi-0.96.0/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_base.py` & `fastapi-0.96.0/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_base_description.py` & `fastapi-0.96.0/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_base_optional.py` & `fastapi-0.96.0/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_basic_optional.py` & `fastapi-0.96.0/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_basic_realm.py` & `fastapi-0.96.0/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_basic_realm_description.py` & `fastapi-0.96.0/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_bearer.py` & `fastapi-0.96.0/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_bearer_description.py` & `fastapi-0.96.0/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_bearer_optional.py` & `fastapi-0.96.0/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_digest.py` & `fastapi-0.96.0/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_digest_description.py` & `fastapi-0.96.0/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_http_digest_optional.py` & `fastapi-0.96.0/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2.py` & `fastapi-0.96.0/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_authorization_code_bearer.py` & `fastapi-0.96.0/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_authorization_code_bearer_description.py` & `fastapi-0.96.0/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_optional.py` & `fastapi-0.96.0/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_optional_description.py` & `fastapi-0.96.0/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_password_bearer_optional.py` & `fastapi-0.96.0/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_oauth2_password_bearer_optional_description.py` & `fastapi-0.96.0/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_openid_connect.py` & `fastapi-0.96.0/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_openid_connect_description.py` & `fastapi-0.96.0/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_security_openid_connect_optional.py` & `fastapi-0.96.0/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_serialize_response.py` & `fastapi-0.96.0/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_serialize_response_dataclass.py` & `fastapi-0.96.0/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_serialize_response_model.py` & `fastapi-0.96.0/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_skip_defaults.py` & `fastapi-0.96.0/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_starlette_exception.py` & `fastapi-0.96.0/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_starlette_urlconvertors.py` & `fastapi-0.96.0/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_sub_callbacks.py` & `fastapi-0.96.0/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_swagger_ui_init_oauth.py` & `fastapi-0.96.0/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tuples.py` & `fastapi-0.96.0/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_typing_python39.py` & `fastapi-0.96.0/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_union_body.py` & `fastapi-0.96.0/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_union_inherited_body.py` & `fastapi-0.96.0/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_validate_response.py` & `fastapi-0.96.0/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_validate_response_dataclass.py` & `fastapi-0.96.0/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_validate_response_recursive.py` & `fastapi-0.96.0/tests/test_validate_response_recursive.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_ws_router.py` & `fastapi-0.96.0/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_modules_same_name_body/test_main.py` & `fastapi-0.96.0/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main.py` & `fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_cors/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `fastapi-0.96.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_events/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extending_openapi/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_metadata/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_metadata/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_params/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_path_params/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py` & `fastapi-0.96.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_templates/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing/test_main.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial001.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial003.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `fastapi-0.96.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/LICENSE` & `fastapi-0.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/README.md` & `fastapi-0.96.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 ## Sponsors
 
 <!-- sponsors -->
 
 <a href="https://cryptapi.io/" target="_blank" title="CryptAPI: Your easy to use, secure and privacy oriented payment gateway."><img src="https://fastapi.tiangolo.com/img/sponsors/cryptapi.svg"></a>
 <a href="https://www.deta.sh/?ref=fastapi" target="_blank" title="The launchpad for all your (team's) ideas"><img src="https://fastapi.tiangolo.com/img/sponsors/deta.svg"></a>
-<a href="https://www.investsuite.com/jobs" target="_blank" title="Wealthtech jobs with FastAPI"><img src="https://fastapi.tiangolo.com/img/sponsors/investsuite.svg"></a>
 <a href="https://training.talkpython.fm/fastapi-courses" target="_blank" title="FastAPI video courses on demand from people you trust"><img src="https://fastapi.tiangolo.com/img/sponsors/talkpython.png"></a>
 <a href="https://testdriven.io/courses/tdd-fastapi/" target="_blank" title="Learn to build high-quality web apps with best practices"><img src="https://fastapi.tiangolo.com/img/sponsors/testdriven.svg"></a>
 <a href="https://github.com/deepset-ai/haystack/" target="_blank" title="Build powerful search from composable, open source building blocks"><img src="https://fastapi.tiangolo.com/img/sponsors/haystack-fastapi.svg"></a>
 <a href="https://careers.powens.com/" target="_blank" title="Powens is hiring!"><img src="https://fastapi.tiangolo.com/img/sponsors/powens.png"></a>
 <a href="https://www.svix.com/" target="_blank" title="Svix - Webhooks as a service"><img src="https://fastapi.tiangolo.com/img/sponsors/svix.svg"></a>
 <a href="https://databento.com/" target="_blank" title="Pay as you go for market data"><img src="https://fastapi.tiangolo.com/img/sponsors/databento.svg"></a>
```

#### html2text {}

```diff
@@ -15,16 +15,15 @@
 duplication. Multiple features from each parameter declaration. Fewer bugs. *
 **Robust**: Get production-ready code. With automatic interactive
 documentation. * **Standards-based**: Based on (and fully compatible with) the
 open standards for APIs: OpenAPI (previously known as Swagger) and JSON_Schema.
 * estimation based on tests on an internal development team, building
 production applications. ## Sponsors  [https://fastapi.tiangolo.com/img/
 sponsors/cryptapi.svg] [https://fastapi.tiangolo.com/img/sponsors/deta.svg]
-[https://fastapi.tiangolo.com/img/sponsors/investsuite.svg] [https://
-fastapi.tiangolo.com/img/sponsors/talkpython.png] [https://
+[https://fastapi.tiangolo.com/img/sponsors/talkpython.png] [https://
 fastapi.tiangolo.com/img/sponsors/testdriven.svg] [https://
 fastapi.tiangolo.com/img/sponsors/haystack-fastapi.svg] [https://
 fastapi.tiangolo.com/img/sponsors/powens.png] [https://fastapi.tiangolo.com/
 img/sponsors/svix.svg] [https://fastapi.tiangolo.com/img/sponsors/
 databento.svg]  Other_sponsors ## Opinions "_[...] I'm using **FastAPI** a ton
 these days. [...] I'm actually planning to use it for all of my team's **ML
 services at Microsoft**. Some of them are getting integrated into the core
```

### Comparing `fastapi-0.95.2/pyproject.toml` & `fastapi-0.96.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-0.95.2/PKG-INFO` & `fastapi-0.96.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi
-Version: 0.95.2
+Version: 0.96.0
 Summary: FastAPI framework, high performance, easy to learn, fast to code, ready for production
 Project-URL: Homepage, https://github.com/tiangolo/fastapi
 Project-URL: Documentation, https://fastapi.tiangolo.com/
 Author-email: Sebastián Ramírez <tiangolo@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -129,15 +129,14 @@
 
 ## Sponsors
 
 <!-- sponsors -->
 
 <a href="https://cryptapi.io/" target="_blank" title="CryptAPI: Your easy to use, secure and privacy oriented payment gateway."><img src="https://fastapi.tiangolo.com/img/sponsors/cryptapi.svg"></a>
 <a href="https://www.deta.sh/?ref=fastapi" target="_blank" title="The launchpad for all your (team's) ideas"><img src="https://fastapi.tiangolo.com/img/sponsors/deta.svg"></a>
-<a href="https://www.investsuite.com/jobs" target="_blank" title="Wealthtech jobs with FastAPI"><img src="https://fastapi.tiangolo.com/img/sponsors/investsuite.svg"></a>
 <a href="https://training.talkpython.fm/fastapi-courses" target="_blank" title="FastAPI video courses on demand from people you trust"><img src="https://fastapi.tiangolo.com/img/sponsors/talkpython.png"></a>
 <a href="https://testdriven.io/courses/tdd-fastapi/" target="_blank" title="Learn to build high-quality web apps with best practices"><img src="https://fastapi.tiangolo.com/img/sponsors/testdriven.svg"></a>
 <a href="https://github.com/deepset-ai/haystack/" target="_blank" title="Build powerful search from composable, open source building blocks"><img src="https://fastapi.tiangolo.com/img/sponsors/haystack-fastapi.svg"></a>
 <a href="https://careers.powens.com/" target="_blank" title="Powens is hiring!"><img src="https://fastapi.tiangolo.com/img/sponsors/powens.png"></a>
 <a href="https://www.svix.com/" target="_blank" title="Svix - Webhooks as a service"><img src="https://fastapi.tiangolo.com/img/sponsors/svix.svg"></a>
 <a href="https://databento.com/" target="_blank" title="Pay as you go for market data"><img src="https://fastapi.tiangolo.com/img/sponsors/databento.svg"></a>
```

