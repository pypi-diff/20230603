# Comparing `tmp/monopyly-1.3.0.tar.gz` & `tmp/monopyly-1.3.1.tar.gz`

## Comparing `monopyly-1.3.0.tar` & `monopyly-1.3.1.tar`

### file list

```diff
@@ -1,202 +1,198 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.3.0/README.md -> monopyly/README.md
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/README.md
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/actions.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/blueprint.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/routes.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/tools.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/__init__.py
--rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/accounts.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/actions.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/banks.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/blueprint.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/forms.py
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/routes.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/transactions.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/cli/run.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/__init__.py
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/transactions.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/__init__.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/_forms.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/fields.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/utils.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/validators.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/default_settings.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/settings.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/__init__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/actions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/blueprint.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/context_processors.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/filters.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/internal_transactions.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/routes.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/accounts.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/actions.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/blueprint.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/cards.py
--rw-r--r--   0        0        0    12008 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/forms.py
--rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/routes.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/statements.py
--rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/transactions.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/__init__.py
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/models.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/preloads.sql
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/schema.sql
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/views.sql
--rw-r--r--   0        0        0    88146 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/jquery-3.4.1.js
--rw-r--r--   0        0        0    47317 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/css/style.css
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/browserconfig.xml
--rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-114.png
--rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-120.png
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-144.png
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-150.png
--rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-152.png
--rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-16.png
--rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-160.png
--rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-180.png
--rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-192.png
--rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-310.png
--rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-32.png
--rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-57.png
--rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-60.png
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-64.png
--rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-70.png
--rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-72.png
--rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-76.png
--rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-96.png
--rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon.ico
--rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon.png
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/statement.png
--rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-account-details.png
--rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-account-summaries.png
--rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-accounts.png
--rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/credit-account-details.png
--rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/credit-transactions.png
--rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/homepage-user.png
--rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/homepage.png
--rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/statement-details.png
--rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/chase-card.png
--rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/discover-card.png
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/new-card.png
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/template-card.png
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-down.png
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-left.png
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-up.png
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/checkmark.png
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-orange-thick.png
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-orange.png
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-thick.png
--rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete.png
--rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/edit.png
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/link.png
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/minus-thick.png
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/minus.png
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/plus-thick.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/plus.png
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/refresh.png
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/save.png
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/sort-asc.png
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/sort-desc.png
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/statement.png
--rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/x-thick.png
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/add_subtransaction.js
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/add_transfer.js
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/autocomplete_transaction.js
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/bind_tag_actions.js
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/define_filter.js
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_account_type_inputs.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_bank_inputs.js
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_credit_account_inputs.js
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_bank.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_bank_account.js
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_transaction.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/flip_card.js
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/infer_card.js
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/infer_statement.js
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/make_payment.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/show_linked_transaction.js
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_account_statement_parameters.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_bank_name.js
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_card_status.js
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_statement_parameters.js
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_statements_display.js
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_transactions_display.js
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/ajax.js
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/autocomplete_input.js
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/expand_box_row.js
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/expand_transaction.js
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_acquisition_form.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_overlays.js
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_subforms.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/update_database_widget.js
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/update_display_ajax.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credits.html
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/index.html
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/layout.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/profile.html
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/story.html
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/auth/login.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/auth/register.html
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_page.html
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summaries.html
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summaries_page.html
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summary.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/accounts_page.html
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_form/account_form.html
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_form/account_form_page_new.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/bank_info_form.html
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transfer_form.html
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/transactions.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/form_page.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transaction_form/subform.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transaction_form/subtransaction_subform.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/subtransactions.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_condensed.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_expanded.html
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transactions.html
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/account_page.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_submission_page.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/cards.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/cards_page.html
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statement_page.html
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statement_summary.html
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statements.html
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statements_page.html
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tags_page.html
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_submission_page.html
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_page.html
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/card_form.html
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/card_form_page_new.html
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_back.html
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_front.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tag_tree/subtag_tree.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tag_tree/tag_tree.html
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/transactions.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.3.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.3.0/COPYING
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.3.0/LICENSE
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monopyly-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 monopyly-1.3.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.3.1/README.md -> monopyly/README.md
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/README.md
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/_version.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/actions.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/blueprint.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/routes.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/tools.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/accounts.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/actions.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/banks.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/blueprint.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/filters.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/forms.py
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/routes.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/transactions.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/cli/run.py
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/transactions.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/utils.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/__init__.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/_forms.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/fields.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/utils.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/validators.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/default_settings.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/settings.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/actions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/blueprint.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/context_processors.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/filters.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/internal_transactions.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/routes.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/accounts.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/actions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/blueprint.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/cards.py
+-rw-r--r--   0        0        0    12008 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/forms.py
+-rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/routes.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/statements.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/transactions.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/__init__.py
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/models.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/preloads.sql
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/schema.sql
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/views.sql
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/css/style.css
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/browserconfig.xml
+-rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-114.png
+-rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-120.png
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-144.png
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-150.png
+-rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-152.png
+-rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-16.png
+-rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-160.png
+-rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-180.png
+-rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-192.png
+-rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-310.png
+-rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-32.png
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-57.png
+-rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-60.png
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-64.png
+-rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-70.png
+-rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-72.png
+-rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-76.png
+-rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-96.png
+-rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon.ico
+-rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon.png
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/statement.png
+-rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-account-details.png
+-rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-account-summaries.png
+-rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-accounts.png
+-rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/credit-account-details.png
+-rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/credit-transactions.png
+-rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/homepage-user.png
+-rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/homepage.png
+-rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/statement-details.png
+-rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/chase-card.png
+-rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/discover-card.png
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/new-card.png
+-rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/template-card.png
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-down.png
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-left.png
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-up.png
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/checkmark.png
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-orange-thick.png
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-orange.png
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-thick.png
+-rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete.png
+-rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/edit.png
+-rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/link.png
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/minus-thick.png
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/minus.png
+-rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/plus-thick.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/plus.png
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/refresh.png
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/save.png
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/sort-asc.png
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/sort-desc.png
+-rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/statement.png
+-rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/x-thick.png
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/add_subtransaction.js
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/add_transfer.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/autocomplete_transaction.js
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/bind_tag_actions.js
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/define_filter.js
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_account_type_inputs.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_bank_inputs.js
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_credit_account_inputs.js
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_bank.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_bank_account.js
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_transaction.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/flip_card.js
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/infer_card.js
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/infer_statement.js
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/make_payment.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/show_linked_transaction.js
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_account_statement_parameters.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_bank_name.js
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_card_status.js
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_statement_parameters.js
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_statements_display.js
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_transactions_display.js
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/ajax.js
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/autocomplete_input.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/expand_box_row.js
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/expand_transaction.js
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_acquisition_form.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_overlays.js
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_subforms.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/update_database_widget.js
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/update_display_ajax.js
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credits.html
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/index.html
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/layout.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/profile.html
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/story.html
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/auth/login.html
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/auth/register.html
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_page.html
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summaries.html
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summaries_page.html
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summary.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/accounts_page.html
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_form/account_form.html
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_form/account_form_page_new.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/bank_info_form.html
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transfer_form.html
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/transactions.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/form_page.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transaction_form/subform.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transaction_form/subtransaction_subform.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_bank_transaction.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_credit_transaction.html
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/subtransactions.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_condensed.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_expanded.html
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transactions.html
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/account_page.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_submission_page.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/cards.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/cards_page.html
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statement_page.html
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statement_summary.html
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statements.html
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statements_page.html
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tags_page.html
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_submission_page.html
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_page.html
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/card_form.html
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/card_form_page_new.html
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_back.html
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_front.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tag_tree/subtag_tree.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tag_tree/tag_tree.html
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/transactions.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.3.1/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.3.1/COPYING
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 monopyly-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 monopyly-1.3.1/PKG-INFO
```

### Comparing `monopyly-1.3.0/monopyly/README.md` & `monopyly-1.3.1/monopyly/README.md`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/__init__.py` & `monopyly-1.3.1/monopyly/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     """
     Register blueprints with the app.
 
     Note
     -----
     Blueprints are imported in this function to avoid loading modules
     that require database models before those models have been set up
-    via `init_app`.
+    via `init_app`. (Rendered obsolete using Authanor; retained in order
+    to keep blueprint imports grouped.)
     """
     # Import blueprints
     from monopyly.auth.blueprint import bp as auth_bp
     from monopyly.banking.blueprint import bp as banking_bp
     from monopyly.core.blueprint import bp as core_bp
     from monopyly.credit.blueprint import bp as credit_bp
```

### Comparing `monopyly-1.3.0/monopyly/auth/routes.py` & `monopyly-1.3.1/monopyly/auth/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Routes for site authentication.
 """
+from authanor.database import db_transaction
 from flask import (
     current_app,
     flash,
     redirect,
     render_template,
     request,
     session,
     url_for,
 )
-from sqlalchemy import insert, select
+from sqlalchemy import select
 from werkzeug.security import check_password_hash, generate_password_hash
 
-from ..database import db_transaction
 from ..database.models import User
 from .actions import get_username_and_password
 from .blueprint import bp
 
 
 @bp.route("/register", methods=("GET", "POST"))
 @db_transaction
```

### Comparing `monopyly-1.3.0/monopyly/auth/tools.py` & `monopyly-1.3.1/monopyly/auth/tools.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/banking/accounts.py` & `monopyly-1.3.1/monopyly/banking/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/banking/actions.py` & `monopyly-1.3.1/monopyly/banking/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/banking/banks.py` & `monopyly-1.3.1/monopyly/banking/banks.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/banking/forms.py` & `monopyly-1.3.1/monopyly/banking/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/banking/routes.py` & `monopyly-1.3.1/monopyly/banking/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Routes for banking financials.
 """
 from itertools import islice
 
+from authanor.database import db_transaction
 from flask import jsonify, redirect, render_template, request, url_for
 
 from ..auth.tools import login_required
 from ..common.forms.utils import extend_field_list_for_ajax
 from ..common.transactions import get_linked_transaction
-from ..database import db_transaction
 from .accounts import BankAccountHandler, BankAccountTypeHandler, save_account
 from .actions import get_bank_account_type_grouping
 from .banks import BankHandler
 from .blueprint import bp
 from .forms import BankAccountForm, BankTransactionForm
 from .transactions import BankTransactionHandler, save_transaction
```

### Comparing `monopyly-1.3.0/monopyly/banking/transactions.py` & `monopyly-1.3.1/monopyly/banking/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,16 @@
         )
         # The transfer is not updated automatically; update it independently
     else:
         # Insert the new transaction into the database
         if transfer_data:
             transfer = record_new_transfer(transfer_data)
             transaction_data.update(
-                internal_transaction_id=transfer.internal_transaction_id
+                internal_transaction_id=transfer.internal_transaction_id,
+                merchant=transfer.account.bank.bank_name,
             )
         transaction = BankTransactionHandler.add_entry(**transaction_data)
     return transaction
 
 
 def record_new_transfer(transfer_data):
     """Record a new transfer given the data for populating the database."""
```

### Comparing `monopyly-1.3.0/monopyly/cli/run.py` & `monopyly-1.3.1/monopyly/cli/run.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/transactions.py` & `monopyly-1.3.1/monopyly/common/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/utils.py` & `monopyly-1.3.1/monopyly/common/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/forms/_forms.py` & `monopyly-1.3.1/monopyly/common/forms/_forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/forms/fields.py` & `monopyly-1.3.1/monopyly/common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/forms/utils.py` & `monopyly-1.3.1/monopyly/common/forms/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/common/forms/validators.py` & `monopyly-1.3.1/monopyly/common/forms/validators.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/config/settings.py` & `monopyly-1.3.1/monopyly/config/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """A module containing objects with various configuration settings."""
-from monopyly.config.default_settings import Config
+from .default_settings import Config
 
 
 class DevelopmentConfig(Config):
     """A configuration object with settings for development."""
 
     DEBUG = True
     SECRET_KEY = "development key"
```

### Comparing `monopyly-1.3.0/monopyly/core/actions.py` & `monopyly-1.3.1/monopyly/core/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/core/context_processors.py` & `monopyly-1.3.1/monopyly/core/context_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .blueprint import bp
 
 
 @bp.app_context_processor
 def inject_global_template_variables():
     """Inject template variablees globally into the template context."""
     template_globals = {
-        "monopyly_version": _display_version(),
+        "app_version": _display_version(),
         "copyright_statement": f"© {date.today().year}",
         "date_today": str(date.today()),
     }
     return template_globals
 
 
 def _display_version():
```

### Comparing `monopyly-1.3.0/monopyly/core/filters.py` & `monopyly-1.3.1/monopyly/core/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/core/routes.py` & `monopyly-1.3.1/monopyly/core/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/accounts.py` & `monopyly-1.3.1/monopyly/credit/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/actions.py` & `monopyly-1.3.1/monopyly/credit/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/cards.py` & `monopyly-1.3.1/monopyly/credit/cards.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/forms.py` & `monopyly-1.3.1/monopyly/credit/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/routes.py` & `monopyly-1.3.1/monopyly/credit/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Routes for credit card financials.
 """
 from itertools import islice
 
+from authanor.database import db_transaction
 from flask import flash, g, jsonify, redirect, render_template, request, url_for
 from sqlalchemy.exc import MultipleResultsFound
 from werkzeug.exceptions import abort
 from wtforms.validators import ValidationError
 
 from ..auth.tools import login_required
 from ..banking.accounts import BankAccountHandler
 from ..banking.banks import BankHandler
 from ..banking.transactions import BankTransactionHandler
 from ..common.forms import form_err_msg
 from ..common.forms.utils import extend_field_list_for_ajax
 from ..common.transactions import get_linked_transaction
 from ..common.utils import dedelimit_float, parse_date, sort_by_frequency
-from ..database import db_transaction
 from .accounts import CreditAccountHandler
 from .actions import (
     get_card_statement_grouping,
     get_potential_preceding_card,
     make_payment,
     transfer_credit_card_statement,
 )
```

### Comparing `monopyly-1.3.0/monopyly/credit/statements.py` & `monopyly-1.3.1/monopyly/credit/statements.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/credit/transactions.py` & `monopyly-1.3.1/monopyly/credit/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/database/__init__.py` & `monopyly-1.3.1/monopyly/database/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Expose commonly used database functionality to the rest of the package.
 """
 import sqlite3
-from functools import wraps
 from pathlib import Path
 
 import click
 from authanor.database import SQLAlchemy as _SQLAlchemy
 from flask import current_app
 from flask.cli import with_appcontext
-from sqlalchemy.schema import Table
 
 from ..core.actions import get_timestamp
 
 DB_NAME = "monopyly.sqlite"
 
 
 class SQLAlchemy(_SQLAlchemy):
@@ -36,47 +34,37 @@
             # Establish a raw connection in order to execute the complete files
             raw_conn = self.engine.raw_connection()
             # Load the tables, table views, and preloaded data
             sql_dir = Path(__file__).parent
             sql_filepaths = [
                 sql_dir / path for path in ("schema.sql", "views.sql", "preloads.sql")
             ]
-            auxiliary_preload_path = app.config["PRELOAD_DATA_PATH"]
+            auxiliary_preload_path = app.config.get("PRELOAD_DATA_PATH")
             if auxiliary_preload_path:
                 sql_filepaths.append(auxiliary_preload_path)
             for sql_filepath in sql_filepaths:
                 with current_app.open_resource(sql_filepath) as sql_file:
                     raw_conn.executescript(sql_file.read().decode("utf8"))
             raw_conn.close()
+        # Top level initialization does not overwrite tables, so it goes at the end
         super().initialize(app)
 
 
 db = SQLAlchemy()
 
 
-def db_transaction(func):
-    """A decorator denoting the wrapped function as a database transaction."""
-
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        with current_app.db.session.begin():
-            return func(*args, **kwargs)
-
-    return wrapper
-
-
 @click.command("init-db")
 @with_appcontext
 def init_db_command():
     """Initialize the database from the command line (if it does not exist)."""
     db_path = current_app.config["DATABASE"]
     if not db_path.is_file():
-        preload_path = current_app.config.get("PRELOAD_DATA_PATH")
         current_app.db.initialize(current_app)
         click.echo(f"Initialized the database ('{db_path}')")
+        preload_path = current_app.config.get("PRELOAD_DATA_PATH")
         if preload_path:
             click.echo(f"Prepopulated the database using '{preload_path}'")
     else:
         click.echo(f"Database exists, using '{db_path}'")
 
 
 @click.command("back-up-db")
```

### Comparing `monopyly-1.3.0/monopyly/database/models.py` & `monopyly-1.3.1/monopyly/database/models.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/database/schema.sql` & `monopyly-1.3.1/monopyly/database/schema.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/database/views.sql` & `monopyly-1.3.1/monopyly/database/views.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/jquery-3.4.1.js` & `monopyly-1.3.1/monopyly/static/jquery-3.7.0.min.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,497 +1,463 @@
-/*! jQuery v3.4.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.7.0 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
-}("undefined" != typeof window ? window : this, function(C, e) {
+}("undefined" != typeof window ? window : this, function(ie, e) {
     "use strict";
-    var t = [],
-        E = C.document,
+    var oe = [],
         r = Object.getPrototypeOf,
-        s = t.slice,
-        g = t.concat,
-        u = t.push,
-        i = t.indexOf,
+        ae = oe.slice,
+        g = oe.flat ? function(e) {
+            return oe.flat.call(e)
+        } : function(e) {
+            return oe.concat.apply([], e)
+        },
+        s = oe.push,
+        se = oe.indexOf,
         n = {},
-        o = n.toString,
-        v = n.hasOwnProperty,
-        a = v.toString,
-        l = a.call(Object),
-        y = {},
-        m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType
+        i = n.toString,
+        ue = n.hasOwnProperty,
+        o = ue.toString,
+        a = o.call(Object),
+        le = {},
+        v = function(e) {
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
         },
-        x = function(e) {
+        y = function(e) {
             return null != e && e === e.window
         },
-        c = {
+        C = ie.document,
+        u = {
             type: !0,
             src: !0,
             nonce: !0,
             noModule: !0
         };
 
-    function b(e, t, n) {
-        var r, i, o = (n = n || E).createElement("script");
+    function m(e, t, n) {
+        var r, i, o = (n = n || C).createElement("script");
         if (o.text = e, t)
-            for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
+            for (r in u)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
-    function w(e) {
-        return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
+    function x(e) {
+        return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[i.call(e)] || "object" : typeof e
     }
-    var f = "3.4.1",
-        k = function(e, t) {
-            return new k.fn.init(e, t)
-        },
-        p = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var t = "3.7.0",
+        l = /HTML$/i,
+        ce = function(e, t) {
+            return new ce.fn.init(e, t)
+        };
 
-    function d(e) {
+    function c(e) {
         var t = !!e && "length" in e && e.length,
-            n = w(e);
-        return !m(e) && !x(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
+            n = x(e);
+        return !v(e) && !y(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
+    }
+
+    function fe(e, t) {
+        return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
-    k.fn = k.prototype = {
-        jquery: f,
-        constructor: k,
+    ce.fn = ce.prototype = {
+        jquery: t,
+        constructor: ce,
         length: 0,
         toArray: function() {
-            return s.call(this)
+            return ae.call(this)
         },
         get: function(e) {
-            return null == e ? s.call(this) : e < 0 ? this[e + this.length] : this[e]
+            return null == e ? ae.call(this) : e < 0 ? this[e + this.length] : this[e]
         },
         pushStack: function(e) {
-            var t = k.merge(this.constructor(), e);
+            var t = ce.merge(this.constructor(), e);
             return t.prevObject = this, t
         },
         each: function(e) {
-            return k.each(this, e)
+            return ce.each(this, e)
         },
         map: function(n) {
-            return this.pushStack(k.map(this, function(e, t) {
+            return this.pushStack(ce.map(this, function(e, t) {
                 return n.call(e, t, e)
             }))
         },
         slice: function() {
-            return this.pushStack(s.apply(this, arguments))
+            return this.pushStack(ae.apply(this, arguments))
         },
         first: function() {
             return this.eq(0)
         },
         last: function() {
             return this.eq(-1)
         },
+        even: function() {
+            return this.pushStack(ce.grep(this, function(e, t) {
+                return (t + 1) % 2
+            }))
+        },
+        odd: function() {
+            return this.pushStack(ce.grep(this, function(e, t) {
+                return t % 2
+            }))
+        },
         eq: function(e) {
             var t = this.length,
                 n = +e + (e < 0 ? t : 0);
             return this.pushStack(0 <= n && n < t ? [this[n]] : [])
         },
         end: function() {
             return this.prevObject || this.constructor()
         },
-        push: u,
-        sort: t.sort,
-        splice: t.splice
-    }, k.extend = k.fn.extend = function() {
+        push: s,
+        sort: oe.sort,
+        splice: oe.splice
+    }, ce.extend = ce.fn.extend = function() {
         var e, t, n, r, i, o, a = arguments[0] || {},
             s = 1,
             u = arguments.length,
             l = !1;
-        for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || m(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
+        for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || v(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
             if (null != (e = arguments[s]))
-                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (k.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || k.isPlainObject(n) ? n : {}, i = !1, a[t] = k.extend(l, o, r)) : void 0 !== r && (a[t] = r));
+                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (ce.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || ce.isPlainObject(n) ? n : {}, i = !1, a[t] = ce.extend(l, o, r)) : void 0 !== r && (a[t] = r));
         return a
-    }, k.extend({
-        expando: "jQuery" + (f + Math.random()).replace(/\D/g, ""),
+    }, ce.extend({
+        expando: "jQuery" + (t + Math.random()).replace(/\D/g, ""),
         isReady: !0,
         error: function(e) {
             throw new Error(e)
         },
         noop: function() {},
         isPlainObject: function(e) {
             var t, n;
-            return !(!e || "[object Object]" !== o.call(e)) && (!(t = r(e)) || "function" == typeof(n = v.call(t, "constructor") && t.constructor) && a.call(n) === l)
+            return !(!e || "[object Object]" !== i.call(e)) && (!(t = r(e)) || "function" == typeof(n = ue.call(t, "constructor") && t.constructor) && o.call(n) === a)
         },
         isEmptyObject: function(e) {
             var t;
             for (t in e) return !1;
             return !0
         },
-        globalEval: function(e, t) {
-            b(e, {
+        globalEval: function(e, t, n) {
+            m(e, {
                 nonce: t && t.nonce
-            })
+            }, n)
         },
         each: function(e, t) {
             var n, r = 0;
-            if (d(e)) {
+            if (c(e)) {
                 for (n = e.length; r < n; r++)
                     if (!1 === t.call(e[r], r, e[r])) break
             } else
                 for (r in e)
                     if (!1 === t.call(e[r], r, e[r])) break;
             return e
         },
-        trim: function(e) {
-            return null == e ? "" : (e + "").replace(p, "")
+        text: function(e) {
+            var t, n = "",
+                r = 0,
+                i = e.nodeType;
+            if (i) {
+                if (1 === i || 9 === i || 11 === i) return e.textContent;
+                if (3 === i || 4 === i) return e.nodeValue
+            } else
+                while (t = e[r++]) n += ce.text(t);
+            return n
         },
         makeArray: function(e, t) {
             var n = t || [];
-            return null != e && (d(Object(e)) ? k.merge(n, "string" == typeof e ? [e] : e) : u.call(n, e)), n
+            return null != e && (c(Object(e)) ? ce.merge(n, "string" == typeof e ? [e] : e) : s.call(n, e)), n
         },
         inArray: function(e, t, n) {
-            return null == t ? -1 : i.call(t, e, n)
+            return null == t ? -1 : se.call(t, e, n)
+        },
+        isXMLDoc: function(e) {
+            var t = e && e.namespaceURI,
+                n = e && (e.ownerDocument || e).documentElement;
+            return !l.test(t || n && n.nodeName || "HTML")
         },
         merge: function(e, t) {
             for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
             return e.length = i, e
         },
         grep: function(e, t, n) {
             for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
             return r
         },
         map: function(e, t, n) {
             var r, i, o = 0,
                 a = [];
-            if (d(e))
+            if (c(e))
                 for (r = e.length; o < r; o++) null != (i = t(e[o], o, n)) && a.push(i);
             else
                 for (o in e) null != (i = t(e[o], o, n)) && a.push(i);
-            return g.apply([], a)
+            return g(a)
         },
         guid: 1,
-        support: y
-    }), "function" == typeof Symbol && (k.fn[Symbol.iterator] = t[Symbol.iterator]), k.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
+        support: le
+    }), "function" == typeof Symbol && (ce.fn[Symbol.iterator] = oe[Symbol.iterator]), ce.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
         n["[object " + t + "]"] = t.toLowerCase()
     });
-    var h = function(n) {
-        var e, d, b, o, i, h, f, g, w, u, l, T, C, a, E, v, s, c, y, k = "sizzle" + 1 * new Date,
-            m = n.document,
-            S = 0,
-            r = 0,
-            p = ue(),
-            x = ue(),
-            N = ue(),
-            A = ue(),
-            D = function(e, t) {
-                return e === t && (l = !0), 0
-            },
-            j = {}.hasOwnProperty,
-            t = [],
-            q = t.pop,
-            L = t.push,
-            H = t.push,
-            O = t.slice,
+    var pe = oe.pop,
+        de = oe.sort,
+        he = oe.splice,
+        ge = "[\\x20\\t\\r\\n\\f]",
+        ve = new RegExp("^" + ge + "+|((?:^|[^\\\\])(?:\\\\.)*)" + ge + "+$", "g");
+    ce.contains = function(e, t) {
+        var n = t && t.parentNode;
+        return e === n || !(!n || 1 !== n.nodeType || !(e.contains ? e.contains(n) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(n)))
+    };
+    var f = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\x80-\uFFFF\w-]/g;
+
+    function p(e, t) {
+        return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
+    }
+    ce.escapeSelector = function(e) {
+        return (e + "").replace(f, p)
+    };
+    var ye = C,
+        me = s;
+    ! function() {
+        var e, b, w, o, a, T, r, C, d, i, k = me,
+            S = ce.expando,
+            E = 0,
+            n = 0,
+            s = W(),
+            c = W(),
+            u = W(),
+            h = W(),
+            l = function(e, t) {
+                return e === t && (a = !0), 0
+            },
+            f = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+            t = "(?:\\\\[\\da-fA-F]{1,6}" + ge + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
+            p = "\\[" + ge + "*(" + t + ")(?:" + ge + "*([*^$|!~]?=)" + ge + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + t + "))|)" + ge + "*\\]",
+            g = ":(" + t + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + p + ")*)|.*)\\)|)",
+            v = new RegExp(ge + "+", "g"),
+            y = new RegExp("^" + ge + "*," + ge + "*"),
+            m = new RegExp("^" + ge + "*([>+~]|" + ge + ")" + ge + "*"),
+            x = new RegExp(ge + "|>"),
+            j = new RegExp(g),
+            A = new RegExp("^" + t + "$"),
+            D = {
+                ID: new RegExp("^#(" + t + ")"),
+                CLASS: new RegExp("^\\.(" + t + ")"),
+                TAG: new RegExp("^(" + t + "|[*])"),
+                ATTR: new RegExp("^" + p),
+                PSEUDO: new RegExp("^" + g),
+                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + ge + "*(even|odd|(([+-]|)(\\d*)n|)" + ge + "*(?:([+-]|)" + ge + "*(\\d+)|))" + ge + "*\\)|)", "i"),
+                bool: new RegExp("^(?:" + f + ")$", "i"),
+                needsContext: new RegExp("^" + ge + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + ge + "*((?:-\\d)?\\d*)" + ge + "*\\)|)(?=[^-]|$)", "i")
+            },
+            N = /^(?:input|select|textarea|button)$/i,
+            q = /^h\d$/i,
+            L = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
+            H = /[+~]/,
+            O = new RegExp("\\\\[\\da-fA-F]{1,6}" + ge + "?|\\\\([^\\r\\n\\f])", "g"),
             P = function(e, t) {
-                for (var n = 0, r = e.length; n < r; n++)
-                    if (e[n] === t) return n;
-                return -1
-            },
-            R = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
-            M = "[\\x20\\t\\r\\n\\f]",
-            I = "(?:\\\\.|[\\w-]|[^\0-\\xa0])+",
-            W = "\\[" + M + "*(" + I + ")(?:" + M + "*([*^$|!~]?=)" + M + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + I + "))|)" + M + "*\\]",
-            $ = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
-            F = new RegExp(M + "+", "g"),
-            B = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
-            _ = new RegExp("^" + M + "*," + M + "*"),
-            z = new RegExp("^" + M + "*([>+~]|" + M + ")" + M + "*"),
-            U = new RegExp(M + "|>"),
-            X = new RegExp($),
-            V = new RegExp("^" + I + "$"),
-            G = {
-                ID: new RegExp("^#(" + I + ")"),
-                CLASS: new RegExp("^\\.(" + I + ")"),
-                TAG: new RegExp("^(" + I + "|[*])"),
-                ATTR: new RegExp("^" + W),
-                PSEUDO: new RegExp("^" + $),
-                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + M + "*(even|odd|(([+-]|)(\\d*)n|)" + M + "*(?:([+-]|)" + M + "*(\\d+)|))" + M + "*\\)|)", "i"),
-                bool: new RegExp("^(?:" + R + ")$", "i"),
-                needsContext: new RegExp("^" + M + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + M + "*((?:-\\d)?\\d*)" + M + "*\\)|)(?=[^-]|$)", "i")
-            },
-            Y = /HTML$/i,
-            Q = /^(?:input|select|textarea|button)$/i,
-            J = /^h\d$/i,
-            K = /^[^{]+\{\s*\[native \w/,
-            Z = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-            ee = /[+~]/,
-            te = new RegExp("\\\\([\\da-f]{1,6}" + M + "?|(" + M + ")|.)", "ig"),
-            ne = function(e, t, n) {
-                var r = "0x" + t - 65536;
-                return r != r || n ? t : r < 0 ? String.fromCharCode(r + 65536) : String.fromCharCode(r >> 10 | 55296, 1023 & r | 56320)
-            },
-            re = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
-            ie = function(e, t) {
-                return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
+                var n = "0x" + e.slice(1) - 65536;
+                return t || (n < 0 ? String.fromCharCode(n + 65536) : String.fromCharCode(n >> 10 | 55296, 1023 & n | 56320))
             },
-            oe = function() {
-                T()
+            R = function() {
+                V()
             },
-            ae = be(function(e) {
-                return !0 === e.disabled && "fieldset" === e.nodeName.toLowerCase()
+            M = J(function(e) {
+                return !0 === e.disabled && fe(e, "fieldset")
             }, {
                 dir: "parentNode",
                 next: "legend"
             });
         try {
-            H.apply(t = O.call(m.childNodes), m.childNodes), t[m.childNodes.length].nodeType
+            k.apply(oe = ae.call(ye.childNodes), ye.childNodes), oe[ye.childNodes.length].nodeType
         } catch (e) {
-            H = {
-                apply: t.length ? function(e, t) {
-                    L.apply(e, O.call(t))
-                } : function(e, t) {
-                    var n = e.length,
-                        r = 0;
-                    while (e[n++] = t[r++]);
-                    e.length = n - 1
+            k = {
+                apply: function(e, t) {
+                    me.apply(e, ae.call(t))
+                },
+                call: function(e) {
+                    me.apply(e, ae.call(arguments, 1))
                 }
             }
         }
 
-        function se(t, e, n, r) {
+        function I(t, e, n, r) {
             var i, o, a, s, u, l, c, f = e && e.ownerDocument,
                 p = e ? e.nodeType : 9;
             if (n = n || [], "string" != typeof t || !t || 1 !== p && 9 !== p && 11 !== p) return n;
-            if (!r && ((e ? e.ownerDocument || e : m) !== C && T(e), e = e || C, E)) {
-                if (11 !== p && (u = Z.exec(t)))
+            if (!r && (V(e), e = e || T, C)) {
+                if (11 !== p && (u = L.exec(t)))
                     if (i = u[1]) {
                         if (9 === p) {
                             if (!(a = e.getElementById(i))) return n;
-                            if (a.id === i) return n.push(a), n
-                        } else if (f && (a = f.getElementById(i)) && y(e, a) && a.id === i) return n.push(a), n
+                            if (a.id === i) return k.call(n, a), n
+                        } else if (f && (a = f.getElementById(i)) && I.contains(e, a) && a.id === i) return k.call(n, a), n
                     } else {
-                        if (u[2]) return H.apply(n, e.getElementsByTagName(t)), n;
-                        if ((i = u[3]) && d.getElementsByClassName && e.getElementsByClassName) return H.apply(n, e.getElementsByClassName(i)), n
-                    } if (d.qsa && !A[t + " "] && (!v || !v.test(t)) && (1 !== p || "object" !== e.nodeName.toLowerCase())) {
-                    if (c = t, f = e, 1 === p && U.test(t)) {
-                        (s = e.getAttribute("id")) ? s = s.replace(re, ie): e.setAttribute("id", s = k), o = (l = h(t)).length;
-                        while (o--) l[o] = "#" + s + " " + xe(l[o]);
-                        c = l.join(","), f = ee.test(t) && ye(e.parentNode) || e
+                        if (u[2]) return k.apply(n, e.getElementsByTagName(t)), n;
+                        if ((i = u[3]) && e.getElementsByClassName) return k.apply(n, e.getElementsByClassName(i)), n
+                    } if (!(h[t + " "] || d && d.test(t))) {
+                    if (c = t, f = e, 1 === p && (x.test(t) || m.test(t))) {
+                        (f = H.test(t) && z(e.parentNode) || e) == e && le.scope || ((s = e.getAttribute("id")) ? s = ce.escapeSelector(s) : e.setAttribute("id", s = S)), o = (l = Y(t)).length;
+                        while (o--) l[o] = (s ? "#" + s : ":scope") + " " + Q(l[o]);
+                        c = l.join(",")
                     }
                     try {
-                        return H.apply(n, f.querySelectorAll(c)), n
+                        return k.apply(n, f.querySelectorAll(c)), n
                     } catch (e) {
-                        A(t, !0)
+                        h(t, !0)
                     } finally {
-                        s === k && e.removeAttribute("id")
+                        s === S && e.removeAttribute("id")
                     }
                 }
             }
-            return g(t.replace(B, "$1"), e, n, r)
+            return re(t.replace(ve, "$1"), e, n, r)
         }
 
-        function ue() {
+        function W() {
             var r = [];
             return function e(t, n) {
                 return r.push(t + " ") > b.cacheLength && delete e[r.shift()], e[t + " "] = n
             }
         }
 
-        function le(e) {
-            return e[k] = !0, e
+        function F(e) {
+            return e[S] = !0, e
         }
 
-        function ce(e) {
-            var t = C.createElement("fieldset");
+        function $(e) {
+            var t = T.createElement("fieldset");
             try {
                 return !!e(t)
             } catch (e) {
                 return !1
             } finally {
                 t.parentNode && t.parentNode.removeChild(t), t = null
             }
         }
 
-        function fe(e, t) {
-            var n = e.split("|"),
-                r = n.length;
-            while (r--) b.attrHandle[n[r]] = t
-        }
-
-        function pe(e, t) {
-            var n = t && e,
-                r = n && 1 === e.nodeType && 1 === t.nodeType && e.sourceIndex - t.sourceIndex;
-            if (r) return r;
-            if (n)
-                while (n = n.nextSibling)
-                    if (n === t) return -1;
-            return e ? 1 : -1
-        }
-
-        function de(t) {
+        function B(t) {
             return function(e) {
-                return "input" === e.nodeName.toLowerCase() && e.type === t
+                return fe(e, "input") && e.type === t
             }
         }
 
-        function he(n) {
+        function _(t) {
             return function(e) {
-                var t = e.nodeName.toLowerCase();
-                return ("input" === t || "button" === t) && e.type === n
+                return (fe(e, "input") || fe(e, "button")) && e.type === t
             }
         }
 
-        function ge(t) {
+        function X(t) {
             return function(e) {
-                return "form" in e ? e.parentNode && !1 === e.disabled ? "label" in e ? "label" in e.parentNode ? e.parentNode.disabled === t : e.disabled === t : e.isDisabled === t || e.isDisabled !== !t && ae(e) === t : e.disabled === t : "label" in e && e.disabled === t
+                return "form" in e ? e.parentNode && !1 === e.disabled ? "label" in e ? "label" in e.parentNode ? e.parentNode.disabled === t : e.disabled === t : e.isDisabled === t || e.isDisabled !== !t && M(e) === t : e.disabled === t : "label" in e && e.disabled === t
             }
         }
 
-        function ve(a) {
-            return le(function(o) {
-                return o = +o, le(function(e, t) {
+        function U(a) {
+            return F(function(o) {
+                return o = +o, F(function(e, t) {
                     var n, r = a([], e.length, o),
                         i = r.length;
                     while (i--) e[n = r[i]] && (e[n] = !(t[n] = e[n]))
                 })
             })
         }
 
-        function ye(e) {
+        function z(e) {
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
-        for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e.namespaceURI,
-                    n = (e.ownerDocument || e).documentElement;
-                return !Y.test(t || n && n.nodeName || "HTML")
-            }, T = se.setDocument = function(e) {
-                var t, n, r = e ? e.ownerDocument || e : m;
-                return r !== C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), m !== C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.attributes = ce(function(e) {
-                    return e.className = "i", !e.getAttribute("className")
-                }), d.getElementsByTagName = ce(function(e) {
-                    return e.appendChild(C.createComment("")), !e.getElementsByTagName("*").length
-                }), d.getElementsByClassName = K.test(C.getElementsByClassName), d.getById = ce(function(e) {
-                    return a.appendChild(e).id = k, !C.getElementsByName || !C.getElementsByName(k).length
-                }), d.getById ? (b.filter.ID = function(e) {
-                    var t = e.replace(te, ne);
-                    return function(e) {
-                        return e.getAttribute("id") === t
-                    }
-                }, b.find.ID = function(e, t) {
-                    if ("undefined" != typeof t.getElementById && E) {
-                        var n = t.getElementById(e);
-                        return n ? [n] : []
-                    }
-                }) : (b.filter.ID = function(e) {
-                    var n = e.replace(te, ne);
-                    return function(e) {
-                        var t = "undefined" != typeof e.getAttributeNode && e.getAttributeNode("id");
-                        return t && t.value === n
-                    }
-                }, b.find.ID = function(e, t) {
-                    if ("undefined" != typeof t.getElementById && E) {
-                        var n, r, i, o = t.getElementById(e);
-                        if (o) {
-                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
-                            i = t.getElementsByName(e), r = 0;
-                            while (o = i[r++])
-                                if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
-                        }
-                        return []
-                    }
-                }), b.find.TAG = d.getElementsByTagName ? function(e, t) {
-                    return "undefined" != typeof t.getElementsByTagName ? t.getElementsByTagName(e) : d.qsa ? t.querySelectorAll(e) : void 0
-                } : function(e, t) {
-                    var n, r = [],
-                        i = 0,
-                        o = t.getElementsByTagName(e);
-                    if ("*" === e) {
-                        while (n = o[i++]) 1 === n.nodeType && r.push(n);
-                        return r
-                    }
-                    return o
-                }, b.find.CLASS = d.getElementsByClassName && function(e, t) {
-                    if ("undefined" != typeof t.getElementsByClassName && E) return t.getElementsByClassName(e)
-                }, s = [], v = [], (d.qsa = K.test(C.querySelectorAll)) && (ce(function(e) {
-                    a.appendChild(e).innerHTML = "<a id='" + k + "'></a><select id='" + k + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && v.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || v.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + k + "-]").length || v.push("~="), e.querySelectorAll(":checked").length || v.push(":checked"), e.querySelectorAll("a#" + k + "+*").length || v.push(".#.+[+~]")
-                }), ce(function(e) {
-                    e.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
-                    var t = C.createElement("input");
-                    t.setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), e.querySelectorAll("[name=d]").length && v.push("name" + M + "*[*^$|!~]?="), 2 !== e.querySelectorAll(":enabled").length && v.push(":enabled", ":disabled"), a.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && v.push(":enabled", ":disabled"), e.querySelectorAll("*,:x"), v.push(",.*:")
-                })), (d.matchesSelector = K.test(c = a.matches || a.webkitMatchesSelector || a.mozMatchesSelector || a.oMatchesSelector || a.msMatchesSelector)) && ce(function(e) {
-                    d.disconnectedMatch = c.call(e, "*"), c.call(e, "[s!='']:x"), s.push("!=", $)
-                }), v = v.length && new RegExp(v.join("|")), s = s.length && new RegExp(s.join("|")), t = K.test(a.compareDocumentPosition), y = t || K.test(a.contains) ? function(e, t) {
-                    var n = 9 === e.nodeType ? e.documentElement : e,
-                        r = t && t.parentNode;
-                    return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
-                } : function(e, t) {
-                    if (t)
-                        while (t = t.parentNode)
-                            if (t === e) return !0;
-                    return !1
-                }, D = t ? function(e, t) {
-                    if (e === t) return l = !0, 0;
-                    var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
-                    return n || (1 & (n = (e.ownerDocument || e) === (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e === C || e.ownerDocument === m && y(m, e) ? -1 : t === C || t.ownerDocument === m && y(m, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
-                } : function(e, t) {
-                    if (e === t) return l = !0, 0;
-                    var n, r = 0,
-                        i = e.parentNode,
-                        o = t.parentNode,
-                        a = [e],
-                        s = [t];
-                    if (!i || !o) return e === C ? -1 : t === C ? 1 : i ? -1 : o ? 1 : u ? P(u, e) - P(u, t) : 0;
-                    if (i === o) return pe(e, t);
-                    n = e;
-                    while (n = n.parentNode) a.unshift(n);
-                    n = t;
-                    while (n = n.parentNode) s.unshift(n);
-                    while (a[r] === s[r]) r++;
-                    return r ? pe(a[r], s[r]) : a[r] === m ? -1 : s[r] === m ? 1 : 0
-                }), C
-            }, se.matches = function(e, t) {
-                return se(e, null, null, t)
-            }, se.matchesSelector = function(e, t) {
-                if ((e.ownerDocument || e) !== C && T(e), d.matchesSelector && E && !A[t + " "] && (!s || !s.test(t)) && (!v || !v.test(t))) try {
-                    var n = c.call(e, t);
-                    if (n || d.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
+
+        function V(e) {
+            var t, n = e ? e.ownerDocument || e : ye;
+            return n != T && 9 === n.nodeType && n.documentElement && (r = (T = n).documentElement, C = !ce.isXMLDoc(T), i = r.matches || r.webkitMatchesSelector || r.msMatchesSelector, ye != T && (t = T.defaultView) && t.top !== t && t.addEventListener("unload", R), le.getById = $(function(e) {
+                return r.appendChild(e).id = ce.expando, !T.getElementsByName || !T.getElementsByName(ce.expando).length
+            }), le.disconnectedMatch = $(function(e) {
+                return i.call(e, "*")
+            }), le.scope = $(function() {
+                return T.querySelectorAll(":scope")
+            }), le.cssHas = $(function() {
+                try {
+                    return T.querySelector(":has(*,:jqfake)"), !1
+                } catch (e) {
+                    return !0
+                }
+            }), le.getById ? (b.filter.ID = function(e) {
+                var t = e.replace(O, P);
+                return function(e) {
+                    return e.getAttribute("id") === t
+                }
+            }, b.find.ID = function(e, t) {
+                if ("undefined" != typeof t.getElementById && C) {
+                    var n = t.getElementById(e);
+                    return n ? [n] : []
+                }
+            }) : (b.filter.ID = function(e) {
+                var n = e.replace(O, P);
+                return function(e) {
+                    var t = "undefined" != typeof e.getAttributeNode && e.getAttributeNode("id");
+                    return t && t.value === n
+                }
+            }, b.find.ID = function(e, t) {
+                if ("undefined" != typeof t.getElementById && C) {
+                    var n, r, i, o = t.getElementById(e);
+                    if (o) {
+                        if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
+                        i = t.getElementsByName(e), r = 0;
+                        while (o = i[r++])
+                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
+                    }
+                    return []
+                }
+            }), b.find.TAG = function(e, t) {
+                return "undefined" != typeof t.getElementsByTagName ? t.getElementsByTagName(e) : t.querySelectorAll(e)
+            }, b.find.CLASS = function(e, t) {
+                if ("undefined" != typeof t.getElementsByClassName && C) return t.getElementsByClassName(e)
+            }, d = [], $(function(e) {
+                var t;
+                r.appendChild(e).innerHTML = "<a id='" + S + "' href='' disabled='disabled'></a><select id='" + S + "-\r\\' disabled='disabled'><option selected=''></option></select>", e.querySelectorAll("[selected]").length || d.push("\\[" + ge + "*(?:value|" + f + ")"), e.querySelectorAll("[id~=" + S + "-]").length || d.push("~="), e.querySelectorAll("a#" + S + "+*").length || d.push(".#.+[+~]"), e.querySelectorAll(":checked").length || d.push(":checked"), (t = T.createElement("input")).setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), r.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && d.push(":enabled", ":disabled"), (t = T.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || d.push("\\[" + ge + "*name" + ge + "*=" + ge + "*(?:''|\"\")")
+            }), le.cssHas || d.push(":has"), d = d.length && new RegExp(d.join("|")), l = function(e, t) {
+                if (e === t) return a = !0, 0;
+                var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
+                return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !le.sortDetached && t.compareDocumentPosition(e) === n ? e === T || e.ownerDocument == ye && I.contains(ye, e) ? -1 : t === T || t.ownerDocument == ye && I.contains(ye, t) ? 1 : o ? se.call(o, e) - se.call(o, t) : 0 : 4 & n ? -1 : 1)
+            }), T
+        }
+        for (e in I.matches = function(e, t) {
+                return I(e, null, null, t)
+            }, I.matchesSelector = function(e, t) {
+                if (V(e), C && !h[t + " "] && (!d || !d.test(t))) try {
+                    var n = i.call(e, t);
+                    if (n || le.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
                 } catch (e) {
-                    A(t, !0)
+                    h(t, !0)
                 }
-                return 0 < se(t, C, null, [e]).length
-            }, se.contains = function(e, t) {
-                return (e.ownerDocument || e) !== C && T(e), y(e, t)
-            }, se.attr = function(e, t) {
-                (e.ownerDocument || e) !== C && T(e);
+                return 0 < I(t, T, null, [e]).length
+            }, I.contains = function(e, t) {
+                return (e.ownerDocument || e) != T && V(e), ce.contains(e, t)
+            }, I.attr = function(e, t) {
+                (e.ownerDocument || e) != T && V(e);
                 var n = b.attrHandle[t.toLowerCase()],
-                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
-                return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
-            }, se.escape = function(e) {
-                return (e + "").replace(re, ie)
-            }, se.error = function(e) {
+                    r = n && ue.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !C) : void 0;
+                return void 0 !== r ? r : e.getAttribute(t)
+            }, I.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
-            }, se.uniqueSort = function(e) {
+            }, ce.uniqueSort = function(e) {
                 var t, n = [],
                     r = 0,
                     i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
+                if (a = !le.sortStable, o = !le.sortStable && ae.call(e, 0), de.call(e, l), a) {
                     while (t = e[i++]) t === e[i] && (r = n.push(i));
-                    while (r--) e.splice(n[r], 1)
+                    while (r--) he.call(e, n[r], 1)
                 }
-                return u = null, e
-            }, o = se.getText = function(e) {
-                var t, n = "",
-                    r = 0,
-                    i = e.nodeType;
-                if (i) {
-                    if (1 === i || 9 === i || 11 === i) {
-                        if ("string" == typeof e.textContent) return e.textContent;
-                        for (e = e.firstChild; e; e = e.nextSibling) n += o(e)
-                    } else if (3 === i || 4 === i) return e.nodeValue
-                } else
-                    while (t = e[r++]) n += o(t);
-                return n
-            }, (b = se.selectors = {
+                return o = null, e
+            }, ce.fn.uniqueSort = function() {
+                return this.pushStack(ce.uniqueSort(ae.apply(this)))
+            }, (b = ce.expr = {
                 cacheLength: 50,
-                createPseudo: le,
-                match: G,
+                createPseudo: F,
+                match: D,
                 attrHandle: {},
                 find: {},
                 relative: {
                     ">": {
                         dir: "parentNode",
                         first: !0
                     },
@@ -504,601 +470,591 @@
                     },
                     "~": {
                         dir: "previousSibling"
                     }
                 },
                 preFilter: {
                     ATTR: function(e) {
-                        return e[1] = e[1].replace(te, ne), e[3] = (e[3] || e[4] || e[5] || "").replace(te, ne), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
+                        return e[1] = e[1].replace(O, P), e[3] = (e[3] || e[4] || e[5] || "").replace(O, P), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
                     },
                     CHILD: function(e) {
-                        return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || se.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && se.error(e[0]), e
+                        return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || I.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && I.error(e[0]), e
                     },
                     PSEUDO: function(e) {
                         var t, n = !e[6] && e[2];
-                        return G.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && X.test(n) && (t = h(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
+                        return D.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && j.test(n) && (t = Y(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
                     }
                 },
                 filter: {
                     TAG: function(e) {
-                        var t = e.replace(te, ne).toLowerCase();
+                        var t = e.replace(O, P).toLowerCase();
                         return "*" === e ? function() {
                             return !0
                         } : function(e) {
-                            return e.nodeName && e.nodeName.toLowerCase() === t
+                            return fe(e, t)
                         }
                     },
                     CLASS: function(e) {
-                        var t = p[e + " "];
-                        return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && p(e, function(e) {
+                        var t = s[e + " "];
+                        return t || (t = new RegExp("(^|" + ge + ")" + e + "(" + ge + "|$)")) && s(e, function(e) {
                             return t.test("string" == typeof e.className && e.className || "undefined" != typeof e.getAttribute && e.getAttribute("class") || "")
                         })
                     },
                     ATTR: function(n, r, i) {
                         return function(e) {
-                            var t = se.attr(e, n);
-                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(F, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
+                            var t = I.attr(e, n);
+                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(v, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
                         }
                     },
-                    CHILD: function(h, e, t, g, v) {
-                        var y = "nth" !== h.slice(0, 3),
-                            m = "last" !== h.slice(-4),
-                            x = "of-type" === e;
-                        return 1 === g && 0 === v ? function(e) {
+                    CHILD: function(d, e, t, h, g) {
+                        var v = "nth" !== d.slice(0, 3),
+                            y = "last" !== d.slice(-4),
+                            m = "of-type" === e;
+                        return 1 === h && 0 === g ? function(e) {
                             return !!e.parentNode
                         } : function(e, t, n) {
-                            var r, i, o, a, s, u, l = y !== m ? "nextSibling" : "previousSibling",
-                                c = e.parentNode,
-                                f = x && e.nodeName.toLowerCase(),
-                                p = !n && !x,
-                                d = !1;
-                            if (c) {
-                                if (y) {
-                                    while (l) {
-                                        a = e;
-                                        while (a = a[l])
-                                            if (x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) return !1;
-                                        u = l = "only" === h && !u && "nextSibling"
+                            var r, i, o, a, s, u = v !== y ? "nextSibling" : "previousSibling",
+                                l = e.parentNode,
+                                c = m && e.nodeName.toLowerCase(),
+                                f = !n && !m,
+                                p = !1;
+                            if (l) {
+                                if (v) {
+                                    while (u) {
+                                        o = e;
+                                        while (o = o[u])
+                                            if (m ? fe(o, c) : 1 === o.nodeType) return !1;
+                                        s = u = "only" === d && !s && "nextSibling"
                                     }
                                     return !0
                                 }
-                                if (u = [m ? c.firstChild : c.lastChild], m && p) {
-                                    d = (s = (r = (i = (o = (a = c)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]) && r[2], a = s && c.childNodes[s];
-                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
-                                        if (1 === a.nodeType && ++d && a === e) {
-                                            i[h] = [S, s, d];
+                                if (s = [y ? l.firstChild : l.lastChild], y && f) {
+                                    p = (a = (r = (i = l[S] || (l[S] = {}))[d] || [])[0] === E && r[1]) && r[2], o = a && l.childNodes[a];
+                                    while (o = ++a && o && o[u] || (p = a = 0) || s.pop())
+                                        if (1 === o.nodeType && ++p && o === e) {
+                                            i[d] = [E, a, p];
                                             break
                                         }
-                                } else if (p && (d = s = (r = (i = (o = (a = e)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]), !1 === d)
-                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
-                                        if ((x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) && ++d && (p && ((i = (o = a[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] = [S, d]), a === e)) break;
-                                return (d -= v) === g || d % g == 0 && 0 <= d / g
+                                } else if (f && (p = a = (r = (i = e[S] || (e[S] = {}))[d] || [])[0] === E && r[1]), !1 === p)
+                                    while (o = ++a && o && o[u] || (p = a = 0) || s.pop())
+                                        if ((m ? fe(o, c) : 1 === o.nodeType) && ++p && (f && ((i = o[S] || (o[S] = {}))[d] = [E, p]), o === e)) break;
+                                return (p -= g) === h || p % h == 0 && 0 <= p / h
                             }
                         }
                     },
                     PSEUDO: function(e, o) {
-                        var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || se.error("unsupported pseudo: " + e);
-                        return a[k] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? le(function(e, t) {
+                        var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || I.error("unsupported pseudo: " + e);
+                        return a[S] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? F(function(e, t) {
                             var n, r = a(e, o),
                                 i = r.length;
-                            while (i--) e[n = P(e, r[i])] = !(t[n] = r[i])
+                            while (i--) e[n = se.call(e, r[i])] = !(t[n] = r[i])
                         }) : function(e) {
                             return a(e, 0, t)
                         }) : a
                     }
                 },
                 pseudos: {
-                    not: le(function(e) {
+                    not: F(function(e) {
                         var r = [],
                             i = [],
-                            s = f(e.replace(B, "$1"));
-                        return s[k] ? le(function(e, t, n, r) {
+                            s = ne(e.replace(ve, "$1"));
+                        return s[S] ? F(function(e, t, n, r) {
                             var i, o = s(e, null, r, []),
                                 a = e.length;
                             while (a--)(i = o[a]) && (e[a] = !(t[a] = i))
                         }) : function(e, t, n) {
                             return r[0] = e, s(r, null, n, i), r[0] = null, !i.pop()
                         }
                     }),
-                    has: le(function(t) {
+                    has: F(function(t) {
                         return function(e) {
-                            return 0 < se(t, e).length
+                            return 0 < I(t, e).length
                         }
                     }),
-                    contains: le(function(t) {
-                        return t = t.replace(te, ne),
+                    contains: F(function(t) {
+                        return t = t.replace(O, P),
                             function(e) {
-                                return -1 < (e.textContent || o(e)).indexOf(t)
+                                return -1 < (e.textContent || ce.text(e)).indexOf(t)
                             }
                     }),
-                    lang: le(function(n) {
-                        return V.test(n || "") || se.error("unsupported lang: " + n), n = n.replace(te, ne).toLowerCase(),
+                    lang: F(function(n) {
+                        return A.test(n || "") || I.error("unsupported lang: " + n), n = n.replace(O, P).toLowerCase(),
                             function(e) {
                                 var t;
                                 do {
-                                    if (t = E ? e.lang : e.getAttribute("xml:lang") || e.getAttribute("lang")) return (t = t.toLowerCase()) === n || 0 === t.indexOf(n + "-")
+                                    if (t = C ? e.lang : e.getAttribute("xml:lang") || e.getAttribute("lang")) return (t = t.toLowerCase()) === n || 0 === t.indexOf(n + "-")
                                 } while ((e = e.parentNode) && 1 === e.nodeType);
                                 return !1
                             }
                     }),
                     target: function(e) {
-                        var t = n.location && n.location.hash;
+                        var t = ie.location && ie.location.hash;
                         return t && t.slice(1) === e.id
                     },
                     root: function(e) {
-                        return e === a
+                        return e === r
                     },
                     focus: function(e) {
-                        return e === C.activeElement && (!C.hasFocus || C.hasFocus()) && !!(e.type || e.href || ~e.tabIndex)
+                        return e === function() {
+                            try {
+                                return T.activeElement
+                            } catch (e) {}
+                        }() && T.hasFocus() && !!(e.type || e.href || ~e.tabIndex)
                     },
-                    enabled: ge(!1),
-                    disabled: ge(!0),
+                    enabled: X(!1),
+                    disabled: X(!0),
                     checked: function(e) {
-                        var t = e.nodeName.toLowerCase();
-                        return "input" === t && !!e.checked || "option" === t && !!e.selected
+                        return fe(e, "input") && !!e.checked || fe(e, "option") && !!e.selected
                     },
                     selected: function(e) {
                         return e.parentNode && e.parentNode.selectedIndex, !0 === e.selected
                     },
                     empty: function(e) {
                         for (e = e.firstChild; e; e = e.nextSibling)
                             if (e.nodeType < 6) return !1;
                         return !0
                     },
                     parent: function(e) {
                         return !b.pseudos.empty(e)
                     },
                     header: function(e) {
-                        return J.test(e.nodeName)
+                        return q.test(e.nodeName)
                     },
                     input: function(e) {
-                        return Q.test(e.nodeName)
+                        return N.test(e.nodeName)
                     },
                     button: function(e) {
-                        var t = e.nodeName.toLowerCase();
-                        return "input" === t && "button" === e.type || "button" === t
+                        return fe(e, "input") && "button" === e.type || fe(e, "button")
                     },
                     text: function(e) {
                         var t;
-                        return "input" === e.nodeName.toLowerCase() && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
+                        return fe(e, "input") && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
                     },
-                    first: ve(function() {
+                    first: U(function() {
                         return [0]
                     }),
-                    last: ve(function(e, t) {
+                    last: U(function(e, t) {
                         return [t - 1]
                     }),
-                    eq: ve(function(e, t, n) {
+                    eq: U(function(e, t, n) {
                         return [n < 0 ? n + t : n]
                     }),
-                    even: ve(function(e, t) {
+                    even: U(function(e, t) {
                         for (var n = 0; n < t; n += 2) e.push(n);
                         return e
                     }),
-                    odd: ve(function(e, t) {
+                    odd: U(function(e, t) {
                         for (var n = 1; n < t; n += 2) e.push(n);
                         return e
                     }),
-                    lt: ve(function(e, t, n) {
-                        for (var r = n < 0 ? n + t : t < n ? t : n; 0 <= --r;) e.push(r);
+                    lt: U(function(e, t, n) {
+                        var r;
+                        for (r = n < 0 ? n + t : t < n ? t : n; 0 <= --r;) e.push(r);
                         return e
                     }),
-                    gt: ve(function(e, t, n) {
+                    gt: U(function(e, t, n) {
                         for (var r = n < 0 ? n + t : n; ++r < t;) e.push(r);
                         return e
                     })
                 }
             }).pseudos.nth = b.pseudos.eq, {
                 radio: !0,
                 checkbox: !0,
                 file: !0,
                 password: !0,
                 image: !0
-            }) b.pseudos[e] = de(e);
+            }) b.pseudos[e] = B(e);
         for (e in {
                 submit: !0,
                 reset: !0
-            }) b.pseudos[e] = he(e);
+            }) b.pseudos[e] = _(e);
 
-        function me() {}
+        function G() {}
 
-        function xe(e) {
+        function Y(e, t) {
+            var n, r, i, o, a, s, u, l = c[e + " "];
+            if (l) return t ? 0 : l.slice(0);
+            a = e, s = [], u = b.preFilter;
+            while (a) {
+                for (o in n && !(r = y.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = m.exec(a)) && (n = r.shift(), i.push({
+                        value: n,
+                        type: r[0].replace(ve, " ")
+                    }), a = a.slice(n.length)), b.filter) !(r = D[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
+                    value: n,
+                    type: o,
+                    matches: r
+                }), a = a.slice(n.length));
+                if (!n) break
+            }
+            return t ? a.length : a ? I.error(e) : c(e, s).slice(0)
+        }
+
+        function Q(e) {
             for (var t = 0, n = e.length, r = ""; t < n; t++) r += e[t].value;
             return r
         }
 
-        function be(s, e, t) {
-            var u = e.dir,
-                l = e.next,
-                c = l || u,
-                f = t && "parentNode" === c,
-                p = r++;
+        function J(a, e, t) {
+            var s = e.dir,
+                u = e.next,
+                l = u || s,
+                c = t && "parentNode" === l,
+                f = n++;
             return e.first ? function(e, t, n) {
-                while (e = e[u])
-                    if (1 === e.nodeType || f) return s(e, t, n);
+                while (e = e[s])
+                    if (1 === e.nodeType || c) return a(e, t, n);
                 return !1
             } : function(e, t, n) {
-                var r, i, o, a = [S, p];
+                var r, i, o = [E, f];
                 if (n) {
-                    while (e = e[u])
-                        if ((1 === e.nodeType || f) && s(e, t, n)) return !0
+                    while (e = e[s])
+                        if ((1 === e.nodeType || c) && a(e, t, n)) return !0
                 } else
-                    while (e = e[u])
-                        if (1 === e.nodeType || f)
-                            if (i = (o = e[k] || (e[k] = {}))[e.uniqueID] || (o[e.uniqueID] = {}), l && l === e.nodeName.toLowerCase()) e = e[u] || e;
+                    while (e = e[s])
+                        if (1 === e.nodeType || c)
+                            if (i = e[S] || (e[S] = {}), u && fe(e, u)) e = e[s] || e;
                             else {
-                                if ((r = i[c]) && r[0] === S && r[1] === p) return a[2] = r[2];
-                                if ((i[c] = a)[2] = s(e, t, n)) return !0
+                                if ((r = i[l]) && r[0] === E && r[1] === f) return o[2] = r[2];
+                                if ((i[l] = o)[2] = a(e, t, n)) return !0
                             } return !1
             }
         }
 
-        function we(i) {
+        function K(i) {
             return 1 < i.length ? function(e, t, n) {
                 var r = i.length;
                 while (r--)
                     if (!i[r](e, t, n)) return !1;
                 return !0
             } : i[0]
         }
 
-        function Te(e, t, n, r, i) {
+        function Z(e, t, n, r, i) {
             for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
             return a
         }
 
-        function Ce(d, h, g, v, y, e) {
-            return v && !v[k] && (v = Ce(v)), y && !y[k] && (y = Ce(y, e)), le(function(e, t, n, r) {
-                var i, o, a, s = [],
-                    u = [],
-                    l = t.length,
-                    c = e || function(e, t, n) {
-                        for (var r = 0, i = t.length; r < i; r++) se(e, t[r], n);
+        function ee(d, h, g, v, y, e) {
+            return v && !v[S] && (v = ee(v)), y && !y[S] && (y = ee(y, e)), F(function(e, t, n, r) {
+                var i, o, a, s, u = [],
+                    l = [],
+                    c = t.length,
+                    f = e || function(e, t, n) {
+                        for (var r = 0, i = t.length; r < i; r++) I(e, t[r], n);
                         return n
                     }(h || "*", n.nodeType ? [n] : n, []),
-                    f = !d || !e && h ? c : Te(c, s, d, n, r),
-                    p = g ? y || (e ? d : l || v) ? [] : t : f;
-                if (g && g(f, p, n, r), v) {
-                    i = Te(p, u), v(i, [], n, r), o = i.length;
-                    while (o--)(a = i[o]) && (p[u[o]] = !(f[u[o]] = a))
+                    p = !d || !e && h ? f : Z(f, u, d, n, r);
+                if (g ? g(p, s = y || (e ? d : c || v) ? [] : t, n, r) : s = p, v) {
+                    i = Z(s, l), v(i, [], n, r), o = i.length;
+                    while (o--)(a = i[o]) && (s[l[o]] = !(p[l[o]] = a))
                 }
                 if (e) {
                     if (y || d) {
                         if (y) {
-                            i = [], o = p.length;
-                            while (o--)(a = p[o]) && i.push(f[o] = a);
-                            y(null, p = [], i, r)
+                            i = [], o = s.length;
+                            while (o--)(a = s[o]) && i.push(p[o] = a);
+                            y(null, s = [], i, r)
                         }
-                        o = p.length;
-                        while (o--)(a = p[o]) && -1 < (i = y ? P(e, a) : s[o]) && (e[i] = !(t[i] = a))
+                        o = s.length;
+                        while (o--)(a = s[o]) && -1 < (i = y ? se.call(e, a) : u[o]) && (e[i] = !(t[i] = a))
                     }
-                } else p = Te(p === t ? p.splice(l, p.length) : p), y ? y(null, t, p, r) : H.apply(t, p)
+                } else s = Z(s === t ? s.splice(c, s.length) : s), y ? y(null, t, s, r) : k.apply(t, s)
             })
         }
 
-        function Ee(e) {
-            for (var i, t, n, r = e.length, o = b.relative[e[0].type], a = o || b.relative[" "], s = o ? 1 : 0, u = be(function(e) {
+        function te(e) {
+            for (var i, t, n, r = e.length, o = b.relative[e[0].type], a = o || b.relative[" "], s = o ? 1 : 0, u = J(function(e) {
                     return e === i
-                }, a, !0), l = be(function(e) {
-                    return -1 < P(i, e)
+                }, a, !0), l = J(function(e) {
+                    return -1 < se.call(i, e)
                 }, a, !0), c = [function(e, t, n) {
-                    var r = !o && (n || t !== w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
+                    var r = !o && (n || t != w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
                     return i = null, r
                 }]; s < r; s++)
-                if (t = b.relative[e[s].type]) c = [be(we(c), t)];
+                if (t = b.relative[e[s].type]) c = [J(K(c), t)];
                 else {
-                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[k]) {
+                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[S]) {
                         for (n = ++s; n < r; n++)
                             if (b.relative[e[n].type]) break;
-                        return Ce(1 < s && we(c), 1 < s && xe(e.slice(0, s - 1).concat({
+                        return ee(1 < s && K(c), 1 < s && Q(e.slice(0, s - 1).concat({
                             value: " " === e[s - 2].type ? "*" : ""
-                        })).replace(B, "$1"), t, s < n && Ee(e.slice(s, n)), n < r && Ee(e = e.slice(n)), n < r && xe(e))
+                        })).replace(ve, "$1"), t, s < n && te(e.slice(s, n)), n < r && te(e = e.slice(n)), n < r && Q(e))
                     }
                     c.push(t)
-                } return we(c)
+                } return K(c)
         }
-        return me.prototype = b.filters = b.pseudos, b.setFilters = new me, h = se.tokenize = function(e, t) {
-            var n, r, i, o, a, s, u, l = x[e + " "];
-            if (l) return t ? 0 : l.slice(0);
-            a = e, s = [], u = b.preFilter;
-            while (a) {
-                for (o in n && !(r = _.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = z.exec(a)) && (n = r.shift(), i.push({
-                        value: n,
-                        type: r[0].replace(B, " ")
-                    }), a = a.slice(n.length)), b.filter) !(r = G[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
-                    value: n,
-                    type: o,
-                    matches: r
-                }), a = a.slice(n.length));
-                if (!n) break
-            }
-            return t ? a.length : a ? se.error(e) : x(e, s).slice(0)
-        }, f = se.compile = function(e, t) {
+
+        function ne(e, t) {
             var n, v, y, m, x, r, i = [],
                 o = [],
-                a = N[e + " "];
+                a = u[e + " "];
             if (!a) {
-                t || (t = h(e)), n = t.length;
-                while (n--)(a = Ee(t[n]))[k] ? i.push(a) : o.push(a);
-                (a = N(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
+                t || (t = Y(e)), n = t.length;
+                while (n--)(a = te(t[n]))[S] ? i.push(a) : o.push(a);
+                (a = u(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
                     var o, a, s, u = 0,
                         l = "0",
                         c = e && [],
                         f = [],
                         p = w,
                         d = e || x && b.find.TAG("*", i),
-                        h = S += null == p ? 1 : Math.random() || .1,
+                        h = E += null == p ? 1 : Math.random() || .1,
                         g = d.length;
-                    for (i && (w = t === C || t || i); l !== g && null != (o = d[l]); l++) {
+                    for (i && (w = t == T || t || i); l !== g && null != (o = d[l]); l++) {
                         if (x && o) {
-                            a = 0, t || o.ownerDocument === C || (T(o), n = !E);
+                            a = 0, t || o.ownerDocument == T || (V(o), n = !C);
                             while (s = v[a++])
-                                if (s(o, t || C, n)) {
-                                    r.push(o);
+                                if (s(o, t || T, n)) {
+                                    k.call(r, o);
                                     break
-                                } i && (S = h)
+                                } i && (E = h)
                         }
                         m && ((o = !s && o) && u--, e && c.push(o))
                     }
                     if (u += l, m && l !== u) {
                         a = 0;
                         while (s = y[a++]) s(c, f, t, n);
                         if (e) {
                             if (0 < u)
-                                while (l--) c[l] || f[l] || (f[l] = q.call(r));
-                            f = Te(f)
+                                while (l--) c[l] || f[l] || (f[l] = pe.call(r));
+                            f = Z(f)
                         }
-                        H.apply(r, f), i && !e && 0 < f.length && 1 < u + y.length && se.uniqueSort(r)
+                        k.apply(r, f), i && !e && 0 < f.length && 1 < u + y.length && ce.uniqueSort(r)
                     }
-                    return i && (S = h, w = p), c
-                }, m ? le(r) : r))).selector = e
+                    return i && (E = h, w = p), c
+                }, m ? F(r) : r))).selector = e
             }
             return a
-        }, g = se.select = function(e, t, n, r) {
+        }
+
+        function re(e, t, n, r) {
             var i, o, a, s, u, l = "function" == typeof e && e,
-                c = !r && h(e = l.selector || e);
+                c = !r && Y(e = l.selector || e);
             if (n = n || [], 1 === c.length) {
-                if (2 < (o = c[0] = c[0].slice(0)).length && "ID" === (a = o[0]).type && 9 === t.nodeType && E && b.relative[o[1].type]) {
-                    if (!(t = (b.find.ID(a.matches[0].replace(te, ne), t) || [])[0])) return n;
+                if (2 < (o = c[0] = c[0].slice(0)).length && "ID" === (a = o[0]).type && 9 === t.nodeType && C && b.relative[o[1].type]) {
+                    if (!(t = (b.find.ID(a.matches[0].replace(O, P), t) || [])[0])) return n;
                     l && (t = t.parentNode), e = e.slice(o.shift().value.length)
                 }
-                i = G.needsContext.test(e) ? 0 : o.length;
+                i = D.needsContext.test(e) ? 0 : o.length;
                 while (i--) {
                     if (a = o[i], b.relative[s = a.type]) break;
-                    if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
-                        if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
+                    if ((u = b.find[s]) && (r = u(a.matches[0].replace(O, P), H.test(o[0].type) && z(t.parentNode) || t))) {
+                        if (o.splice(i, 1), !(e = r.length && Q(o))) return k.apply(n, r), n;
                         break
                     }
                 }
             }
-            return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = k.split("").sort(D).join("") === k, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
-            return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
-        }), ce(function(e) {
-            return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
-        }) || fe("type|href|height|width", function(e, t, n) {
-            if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
-        }), d.attributes && ce(function(e) {
-            return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
-        }) || fe("value", function(e, t, n) {
-            if (!n && "input" === e.nodeName.toLowerCase()) return e.defaultValue
-        }), ce(function(e) {
-            return null == e.getAttribute("disabled")
-        }) || fe(R, function(e, t, n) {
-            var r;
-            if (!n) return !0 === e[t] ? t.toLowerCase() : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
-        }), se
-    }(C);
-    k.find = h, k.expr = h.selectors, k.expr[":"] = k.expr.pseudos, k.uniqueSort = k.unique = h.uniqueSort, k.text = h.getText, k.isXMLDoc = h.isXML, k.contains = h.contains, k.escapeSelector = h.escape;
-    var T = function(e, t, n) {
+            return (l || ne(e, c))(r, t, !C, n, !t || H.test(e) && z(t.parentNode) || t), n
+        }
+        G.prototype = b.filters = b.pseudos, b.setFilters = new G, le.sortStable = S.split("").sort(l).join("") === S, V(), le.sortDetached = $(function(e) {
+            return 1 & e.compareDocumentPosition(T.createElement("fieldset"))
+        }), ce.find = I, ce.expr[":"] = ce.expr.pseudos, ce.unique = ce.uniqueSort, I.compile = ne, I.select = re, I.setDocument = V, I.escape = ce.escapeSelector, I.getText = ce.text, I.isXML = ce.isXMLDoc, I.selectors = ce.expr, I.support = ce.support, I.uniqueSort = ce.uniqueSort
+    }();
+    var d = function(e, t, n) {
             var r = [],
                 i = void 0 !== n;
             while ((e = e[t]) && 9 !== e.nodeType)
                 if (1 === e.nodeType) {
-                    if (i && k(e).is(n)) break;
+                    if (i && ce(e).is(n)) break;
                     r.push(e)
                 } return r
         },
-        S = function(e, t) {
+        h = function(e, t) {
             for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
             return n
         },
-        N = k.expr.match.needsContext;
+        b = ce.expr.match.needsContext,
+        w = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function A(e, t) {
-        return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
-    }
-    var D = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
-
-    function j(e, n, r) {
-        return m(n) ? k.grep(e, function(e, t) {
+    function T(e, n, r) {
+        return v(n) ? ce.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
-        }) : n.nodeType ? k.grep(e, function(e) {
+        }) : n.nodeType ? ce.grep(e, function(e) {
             return e === n !== r
-        }) : "string" != typeof n ? k.grep(e, function(e) {
-            return -1 < i.call(n, e) !== r
-        }) : k.filter(n, e, r)
+        }) : "string" != typeof n ? ce.grep(e, function(e) {
+            return -1 < se.call(n, e) !== r
+        }) : ce.filter(n, e, r)
     }
-    k.filter = function(e, t, n) {
+    ce.filter = function(e, t, n) {
         var r = t[0];
-        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? k.find.matchesSelector(r, e) ? [r] : [] : k.find.matches(e, k.grep(t, function(e) {
+        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? ce.find.matchesSelector(r, e) ? [r] : [] : ce.find.matches(e, ce.grep(t, function(e) {
             return 1 === e.nodeType
         }))
-    }, k.fn.extend({
+    }, ce.fn.extend({
         find: function(e) {
             var t, n, r = this.length,
                 i = this;
-            if ("string" != typeof e) return this.pushStack(k(e).filter(function() {
+            if ("string" != typeof e) return this.pushStack(ce(e).filter(function() {
                 for (t = 0; t < r; t++)
-                    if (k.contains(i[t], this)) return !0
+                    if (ce.contains(i[t], this)) return !0
             }));
-            for (n = this.pushStack([]), t = 0; t < r; t++) k.find(e, i[t], n);
-            return 1 < r ? k.uniqueSort(n) : n
+            for (n = this.pushStack([]), t = 0; t < r; t++) ce.find(e, i[t], n);
+            return 1 < r ? ce.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(j(this, e || [], !1))
+            return this.pushStack(T(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(j(this, e || [], !0))
+            return this.pushStack(T(this, e || [], !0))
         },
         is: function(e) {
-            return !!j(this, "string" == typeof e && N.test(e) ? k(e) : e || [], !1).length
+            return !!T(this, "string" == typeof e && b.test(e) ? ce(e) : e || [], !1).length
         }
     });
-    var q, L = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
-    (k.fn.init = function(e, t, n) {
+    var k, S = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    (ce.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || q, "string" == typeof e) {
-            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : L.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
+        if (n = n || k, "string" == typeof e) {
+            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : S.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
-                if (t = t instanceof k ? t[0] : t, k.merge(this, k.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), D.test(r[1]) && k.isPlainObject(t))
-                    for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
+                if (t = t instanceof ce ? t[0] : t, ce.merge(this, ce.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : C, !0)), w.test(r[1]) && ce.isPlainObject(t))
+                    for (r in t) v(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
-            return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
+            return (i = C.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
-        return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(k) : k.makeArray(e, this)
-    }).prototype = k.fn, q = k(E);
-    var H = /^(?:parents|prev(?:Until|All))/,
-        O = {
+        return e.nodeType ? (this[0] = e, this.length = 1, this) : v(e) ? void 0 !== n.ready ? n.ready(e) : e(ce) : ce.makeArray(e, this)
+    }).prototype = ce.fn, k = ce(C);
+    var E = /^(?:parents|prev(?:Until|All))/,
+        j = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
 
-    function P(e, t) {
+    function A(e, t) {
         while ((e = e[t]) && 1 !== e.nodeType);
         return e
     }
-    k.fn.extend({
+    ce.fn.extend({
         has: function(e) {
-            var t = k(e, this),
+            var t = ce(e, this),
                 n = t.length;
             return this.filter(function() {
                 for (var e = 0; e < n; e++)
-                    if (k.contains(this, t[e])) return !0
+                    if (ce.contains(this, t[e])) return !0
             })
         },
         closest: function(e, t) {
             var n, r = 0,
                 i = this.length,
                 o = [],
-                a = "string" != typeof e && k(e);
-            if (!N.test(e))
+                a = "string" != typeof e && ce(e);
+            if (!b.test(e))
                 for (; r < i; r++)
                     for (n = this[r]; n && n !== t; n = n.parentNode)
-                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && k.find.matchesSelector(n, e))) {
+                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && ce.find.matchesSelector(n, e))) {
                             o.push(n);
                             break
-                        } return this.pushStack(1 < o.length ? k.uniqueSort(o) : o)
+                        } return this.pushStack(1 < o.length ? ce.uniqueSort(o) : o)
         },
         index: function(e) {
-            return e ? "string" == typeof e ? i.call(k(e), this[0]) : i.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+            return e ? "string" == typeof e ? se.call(ce(e), this[0]) : se.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
         },
         add: function(e, t) {
-            return this.pushStack(k.uniqueSort(k.merge(this.get(), k(e, t))))
+            return this.pushStack(ce.uniqueSort(ce.merge(this.get(), ce(e, t))))
         },
         addBack: function(e) {
             return this.add(null == e ? this.prevObject : this.prevObject.filter(e))
         }
-    }), k.each({
+    }), ce.each({
         parent: function(e) {
             var t = e.parentNode;
             return t && 11 !== t.nodeType ? t : null
         },
         parents: function(e) {
-            return T(e, "parentNode")
+            return d(e, "parentNode")
         },
         parentsUntil: function(e, t, n) {
-            return T(e, "parentNode", n)
+            return d(e, "parentNode", n)
         },
         next: function(e) {
-            return P(e, "nextSibling")
+            return A(e, "nextSibling")
         },
         prev: function(e) {
-            return P(e, "previousSibling")
+            return A(e, "previousSibling")
         },
         nextAll: function(e) {
-            return T(e, "nextSibling")
+            return d(e, "nextSibling")
         },
         prevAll: function(e) {
-            return T(e, "previousSibling")
+            return d(e, "previousSibling")
         },
         nextUntil: function(e, t, n) {
-            return T(e, "nextSibling", n)
+            return d(e, "nextSibling", n)
         },
         prevUntil: function(e, t, n) {
-            return T(e, "previousSibling", n)
+            return d(e, "previousSibling", n)
         },
         siblings: function(e) {
-            return S((e.parentNode || {}).firstChild, e)
+            return h((e.parentNode || {}).firstChild, e)
         },
         children: function(e) {
-            return S(e.firstChild)
+            return h(e.firstChild)
         },
         contents: function(e) {
-            return "undefined" != typeof e.contentDocument ? e.contentDocument : (A(e, "template") && (e = e.content || e), k.merge([], e.childNodes))
+            return null != e.contentDocument && r(e.contentDocument) ? e.contentDocument : (fe(e, "template") && (e = e.content || e), ce.merge([], e.childNodes))
         }
     }, function(r, i) {
-        k.fn[r] = function(e, t) {
-            var n = k.map(this, i, e);
-            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = k.filter(t, n)), 1 < this.length && (O[r] || k.uniqueSort(n), H.test(r) && n.reverse()), this.pushStack(n)
+        ce.fn[r] = function(e, t) {
+            var n = ce.map(this, i, e);
+            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = ce.filter(t, n)), 1 < this.length && (j[r] || ce.uniqueSort(n), E.test(r) && n.reverse()), this.pushStack(n)
         }
     });
-    var R = /[^\x20\t\r\n\f]+/g;
+    var D = /[^\x20\t\r\n\f]+/g;
 
-    function M(e) {
+    function N(e) {
         return e
     }
 
-    function I(e) {
+    function q(e) {
         throw e
     }
 
-    function W(e, t, n, r) {
+    function L(e, t, n, r) {
         var i;
         try {
-            e && m(i = e.promise) ? i.call(e).done(t).fail(n) : e && m(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
+            e && v(i = e.promise) ? i.call(e).done(t).fail(n) : e && v(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
         } catch (e) {
             n.apply(void 0, [e])
         }
     }
-    k.Callbacks = function(r) {
+    ce.Callbacks = function(r) {
         var e, n;
-        r = "string" == typeof r ? (e = r, n = {}, k.each(e.match(R) || [], function(e, t) {
+        r = "string" == typeof r ? (e = r, n = {}, ce.each(e.match(D) || [], function(e, t) {
             n[t] = !0
-        }), n) : k.extend({}, r);
+        }), n) : ce.extend({}, r);
         var i, t, o, a, s = [],
             u = [],
             l = -1,
             c = function() {
                 for (a = a || r.once, o = i = !0; u.length; l = -1) {
                     t = u.shift();
                     while (++l < s.length) !1 === s[l].apply(t[0], t[1]) && r.stopOnFalse && (l = s.length, t = !1)
                 }
                 r.memory || (t = !1), i = !1, a && (s = t ? [] : "")
             },
             f = {
                 add: function() {
                     return s && (t && !i && (l = s.length - 1, u.push(t)), function n(e) {
-                        k.each(e, function(e, t) {
-                            m(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== w(t) && n(t)
+                        ce.each(e, function(e, t) {
+                            v(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== x(t) && n(t)
                         })
                     }(arguments), t && !i && c()), this
                 },
                 remove: function() {
-                    return k.each(arguments, function(e, t) {
+                    return ce.each(arguments, function(e, t) {
                         var n;
-                        while (-1 < (n = k.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
+                        while (-1 < (n = ce.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
                     }), this
                 },
                 has: function(e) {
-                    return e ? -1 < k.inArray(e, s) : 0 < s.length
+                    return e ? -1 < ce.inArray(e, s) : 0 < s.length
                 },
                 empty: function() {
                     return s && (s = []), this
                 },
                 disable: function() {
                     return a = u = [], s = t = "", this
                 },
@@ -1118,40 +1074,40 @@
                     return f.fireWith(this, arguments), this
                 },
                 fired: function() {
                     return !!o
                 }
             };
         return f
-    }, k.extend({
+    }, ce.extend({
         Deferred: function(e) {
             var o = [
-                    ["notify", "progress", k.Callbacks("memory"), k.Callbacks("memory"), 2],
-                    ["resolve", "done", k.Callbacks("once memory"), k.Callbacks("once memory"), 0, "resolved"],
-                    ["reject", "fail", k.Callbacks("once memory"), k.Callbacks("once memory"), 1, "rejected"]
+                    ["notify", "progress", ce.Callbacks("memory"), ce.Callbacks("memory"), 2],
+                    ["resolve", "done", ce.Callbacks("once memory"), ce.Callbacks("once memory"), 0, "resolved"],
+                    ["reject", "fail", ce.Callbacks("once memory"), ce.Callbacks("once memory"), 1, "rejected"]
                 ],
                 i = "pending",
                 a = {
                     state: function() {
                         return i
                     },
                     always: function() {
                         return s.done(arguments).fail(arguments), this
                     },
                     "catch": function(e) {
                         return a.then(null, e)
                     },
                     pipe: function() {
                         var i = arguments;
-                        return k.Deferred(function(r) {
-                            k.each(o, function(e, t) {
-                                var n = m(i[t[4]]) && i[t[4]];
+                        return ce.Deferred(function(r) {
+                            ce.each(o, function(e, t) {
+                                var n = v(i[t[4]]) && i[t[4]];
                                 s[t[1]](function() {
                                     var e = n && n.apply(this, arguments);
-                                    e && m(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
+                                    e && v(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
                                 })
                             }), i = null
                         }).promise()
                     },
                     then: function(t, n, r) {
                         var u = 0;
 
@@ -1159,483 +1115,464 @@
                             return function() {
                                 var n = this,
                                     r = arguments,
                                     e = function() {
                                         var e, t;
                                         if (!(i < u)) {
                                             if ((e = a.apply(n, r)) === o.promise()) throw new TypeError("Thenable self-resolution");
-                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, m(t) ? s ? t.call(e, l(u, o, M, s), l(u, o, I, s)) : (u++, t.call(e, l(u, o, M, s), l(u, o, I, s), l(u, o, M, o.notifyWith))) : (a !== M && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
+                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, v(t) ? s ? t.call(e, l(u, o, N, s), l(u, o, q, s)) : (u++, t.call(e, l(u, o, N, s), l(u, o, q, s), l(u, o, N, o.notifyWith))) : (a !== N && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
                                         }
                                     },
                                     t = s ? e : function() {
                                         try {
                                             e()
                                         } catch (e) {
-                                            k.Deferred.exceptionHook && k.Deferred.exceptionHook(e, t.stackTrace), u <= i + 1 && (a !== I && (n = void 0, r = [e]), o.rejectWith(n, r))
+                                            ce.Deferred.exceptionHook && ce.Deferred.exceptionHook(e, t.error), u <= i + 1 && (a !== q && (n = void 0, r = [e]), o.rejectWith(n, r))
                                         }
                                     };
-                                i ? t() : (k.Deferred.getStackHook && (t.stackTrace = k.Deferred.getStackHook()), C.setTimeout(t))
+                                i ? t() : (ce.Deferred.getErrorHook ? t.error = ce.Deferred.getErrorHook() : ce.Deferred.getStackHook && (t.error = ce.Deferred.getStackHook()), ie.setTimeout(t))
                             }
                         }
-                        return k.Deferred(function(e) {
-                            o[0][3].add(l(0, e, m(r) ? r : M, e.notifyWith)), o[1][3].add(l(0, e, m(t) ? t : M)), o[2][3].add(l(0, e, m(n) ? n : I))
+                        return ce.Deferred(function(e) {
+                            o[0][3].add(l(0, e, v(r) ? r : N, e.notifyWith)), o[1][3].add(l(0, e, v(t) ? t : N)), o[2][3].add(l(0, e, v(n) ? n : q))
                         }).promise()
                     },
                     promise: function(e) {
-                        return null != e ? k.extend(e, a) : a
+                        return null != e ? ce.extend(e, a) : a
                     }
                 },
                 s = {};
-            return k.each(o, function(e, t) {
+            return ce.each(o, function(e, t) {
                 var n = t[2],
                     r = t[5];
                 a[t[1]] = n.add, r && n.add(function() {
                     i = r
                 }, o[3 - e][2].disable, o[3 - e][3].disable, o[0][2].lock, o[0][3].lock), n.add(t[3].fire), s[t[0]] = function() {
                     return s[t[0] + "With"](this === s ? void 0 : this, arguments), this
                 }, s[t[0] + "With"] = n.fireWith
             }), a.promise(s), e && e.call(s, s), s
         },
         when: function(e) {
             var n = arguments.length,
                 t = n,
                 r = Array(t),
-                i = s.call(arguments),
-                o = k.Deferred(),
+                i = ae.call(arguments),
+                o = ce.Deferred(),
                 a = function(t) {
                     return function(e) {
-                        r[t] = this, i[t] = 1 < arguments.length ? s.call(arguments) : e, --n || o.resolveWith(r, i)
+                        r[t] = this, i[t] = 1 < arguments.length ? ae.call(arguments) : e, --n || o.resolveWith(r, i)
                     }
                 };
-            if (n <= 1 && (W(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || m(i[t] && i[t].then))) return o.then();
-            while (t--) W(i[t], a(t), o.reject);
+            if (n <= 1 && (L(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || v(i[t] && i[t].then))) return o.then();
+            while (t--) L(i[t], a(t), o.reject);
             return o.promise()
         }
     });
-    var $ = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
-    k.Deferred.exceptionHook = function(e, t) {
-        C.console && C.console.warn && e && $.test(e.name) && C.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
-    }, k.readyException = function(e) {
-        C.setTimeout(function() {
+    var H = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+    ce.Deferred.exceptionHook = function(e, t) {
+        ie.console && ie.console.warn && e && H.test(e.name) && ie.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
+    }, ce.readyException = function(e) {
+        ie.setTimeout(function() {
             throw e
         })
     };
-    var F = k.Deferred();
+    var O = ce.Deferred();
 
-    function B() {
-        E.removeEventListener("DOMContentLoaded", B), C.removeEventListener("load", B), k.ready()
+    function P() {
+        C.removeEventListener("DOMContentLoaded", P), ie.removeEventListener("load", P), ce.ready()
     }
-    k.fn.ready = function(e) {
-        return F.then(e)["catch"](function(e) {
-            k.readyException(e)
+    ce.fn.ready = function(e) {
+        return O.then(e)["catch"](function(e) {
+            ce.readyException(e)
         }), this
-    }, k.extend({
+    }, ce.extend({
         isReady: !1,
         readyWait: 1,
         ready: function(e) {
-            (!0 === e ? --k.readyWait : k.isReady) || (k.isReady = !0) !== e && 0 < --k.readyWait || F.resolveWith(E, [k])
+            (!0 === e ? --ce.readyWait : ce.isReady) || (ce.isReady = !0) !== e && 0 < --ce.readyWait || O.resolveWith(C, [ce])
         }
-    }), k.ready.then = F.then, "complete" === E.readyState || "loading" !== E.readyState && !E.documentElement.doScroll ? C.setTimeout(k.ready) : (E.addEventListener("DOMContentLoaded", B), C.addEventListener("load", B));
-    var _ = function(e, t, n, r, i, o, a) {
+    }), ce.ready.then = O.then, "complete" === C.readyState || "loading" !== C.readyState && !C.documentElement.doScroll ? ie.setTimeout(ce.ready) : (C.addEventListener("DOMContentLoaded", P), ie.addEventListener("load", P));
+    var R = function(e, t, n, r, i, o, a) {
             var s = 0,
                 u = e.length,
                 l = null == n;
-            if ("object" === w(n))
-                for (s in i = !0, n) _(e, t, s, n[s], !0, o, a);
-            else if (void 0 !== r && (i = !0, m(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
-                    return l.call(k(e), n)
+            if ("object" === x(n))
+                for (s in i = !0, n) R(e, t, s, n[s], !0, o, a);
+            else if (void 0 !== r && (i = !0, v(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
+                    return l.call(ce(e), n)
                 })), t))
                 for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
             return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
         },
-        z = /^-ms-/,
-        U = /-([a-z])/g;
+        M = /^-ms-/,
+        I = /-([a-z])/g;
 
-    function X(e, t) {
+    function W(e, t) {
         return t.toUpperCase()
     }
 
-    function V(e) {
-        return e.replace(z, "ms-").replace(U, X)
+    function F(e) {
+        return e.replace(M, "ms-").replace(I, W)
     }
-    var G = function(e) {
+    var $ = function(e) {
         return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
     };
 
-    function Y() {
-        this.expando = k.expando + Y.uid++
+    function B() {
+        this.expando = ce.expando + B.uid++
     }
-    Y.uid = 1, Y.prototype = {
+    B.uid = 1, B.prototype = {
         cache: function(e) {
             var t = e[this.expando];
-            return t || (t = {}, G(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
+            return t || (t = {}, $(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
                 value: t,
                 configurable: !0
             }))), t
         },
         set: function(e, t, n) {
             var r, i = this.cache(e);
-            if ("string" == typeof t) i[V(t)] = n;
+            if ("string" == typeof t) i[F(t)] = n;
             else
-                for (r in t) i[V(r)] = t[r];
+                for (r in t) i[F(r)] = t[r];
             return i
         },
         get: function(e, t) {
-            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][V(t)]
+            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][F(t)]
         },
         access: function(e, t, n) {
             return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
         },
         remove: function(e, t) {
             var n, r = e[this.expando];
             if (void 0 !== r) {
                 if (void 0 !== t) {
-                    n = (t = Array.isArray(t) ? t.map(V) : (t = V(t)) in r ? [t] : t.match(R) || []).length;
+                    n = (t = Array.isArray(t) ? t.map(F) : (t = F(t)) in r ? [t] : t.match(D) || []).length;
                     while (n--) delete r[t[n]]
-                }(void 0 === t || k.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
+                }(void 0 === t || ce.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
             }
         },
         hasData: function(e) {
             var t = e[this.expando];
-            return void 0 !== t && !k.isEmptyObject(t)
+            return void 0 !== t && !ce.isEmptyObject(t)
         }
     };
-    var Q = new Y,
-        J = new Y,
-        K = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        Z = /[A-Z]/g;
+    var _ = new B,
+        X = new B,
+        U = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        z = /[A-Z]/g;
 
-    function ee(e, t, n) {
+    function V(e, t, n) {
         var r, i;
         if (void 0 === n && 1 === e.nodeType)
-            if (r = "data-" + t.replace(Z, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
+            if (r = "data-" + t.replace(z, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
                 try {
-                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : K.test(i) ? JSON.parse(i) : i)
+                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : U.test(i) ? JSON.parse(i) : i)
                 } catch (e) {}
-                J.set(e, t, n)
+                X.set(e, t, n)
             } else n = void 0;
         return n
     }
-    k.extend({
+    ce.extend({
         hasData: function(e) {
-            return J.hasData(e) || Q.hasData(e)
+            return X.hasData(e) || _.hasData(e)
         },
         data: function(e, t, n) {
-            return J.access(e, t, n)
+            return X.access(e, t, n)
         },
         removeData: function(e, t) {
-            J.remove(e, t)
+            X.remove(e, t)
         },
         _data: function(e, t, n) {
-            return Q.access(e, t, n)
+            return _.access(e, t, n)
         },
         _removeData: function(e, t) {
-            Q.remove(e, t)
+            _.remove(e, t)
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         data: function(n, e) {
             var t, r, i, o = this[0],
                 a = o && o.attributes;
             if (void 0 === n) {
-                if (this.length && (i = J.get(o), 1 === o.nodeType && !Q.get(o, "hasDataAttrs"))) {
+                if (this.length && (i = X.get(o), 1 === o.nodeType && !_.get(o, "hasDataAttrs"))) {
                     t = a.length;
-                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = V(r.slice(5)), ee(o, r, i[r]));
-                    Q.set(o, "hasDataAttrs", !0)
+                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = F(r.slice(5)), V(o, r, i[r]));
+                    _.set(o, "hasDataAttrs", !0)
                 }
                 return i
             }
             return "object" == typeof n ? this.each(function() {
-                J.set(this, n)
-            }) : _(this, function(e) {
+                X.set(this, n)
+            }) : R(this, function(e) {
                 var t;
-                if (o && void 0 === e) return void 0 !== (t = J.get(o, n)) ? t : void 0 !== (t = ee(o, n)) ? t : void 0;
+                if (o && void 0 === e) return void 0 !== (t = X.get(o, n)) ? t : void 0 !== (t = V(o, n)) ? t : void 0;
                 this.each(function() {
-                    J.set(this, n, e)
+                    X.set(this, n, e)
                 })
             }, null, e, 1 < arguments.length, null, !0)
         },
         removeData: function(e) {
             return this.each(function() {
-                J.remove(this, e)
+                X.remove(this, e)
             })
         }
-    }), k.extend({
+    }), ce.extend({
         queue: function(e, t, n) {
             var r;
-            if (e) return t = (t || "fx") + "queue", r = Q.get(e, t), n && (!r || Array.isArray(n) ? r = Q.access(e, t, k.makeArray(n)) : r.push(n)), r || []
+            if (e) return t = (t || "fx") + "queue", r = _.get(e, t), n && (!r || Array.isArray(n) ? r = _.access(e, t, ce.makeArray(n)) : r.push(n)), r || []
         },
         dequeue: function(e, t) {
             t = t || "fx";
-            var n = k.queue(e, t),
+            var n = ce.queue(e, t),
                 r = n.length,
                 i = n.shift(),
-                o = k._queueHooks(e, t);
+                o = ce._queueHooks(e, t);
             "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, function() {
-                k.dequeue(e, t)
+                ce.dequeue(e, t)
             }, o)), !r && o && o.empty.fire()
         },
         _queueHooks: function(e, t) {
             var n = t + "queueHooks";
-            return Q.get(e, n) || Q.access(e, n, {
-                empty: k.Callbacks("once memory").add(function() {
-                    Q.remove(e, [t + "queue", n])
+            return _.get(e, n) || _.access(e, n, {
+                empty: ce.Callbacks("once memory").add(function() {
+                    _.remove(e, [t + "queue", n])
                 })
             })
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         queue: function(t, n) {
             var e = 2;
-            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? k.queue(this[0], t) : void 0 === n ? this : this.each(function() {
-                var e = k.queue(this, t, n);
-                k._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && k.dequeue(this, t)
+            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? ce.queue(this[0], t) : void 0 === n ? this : this.each(function() {
+                var e = ce.queue(this, t, n);
+                ce._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && ce.dequeue(this, t)
             })
         },
         dequeue: function(e) {
             return this.each(function() {
-                k.dequeue(this, e)
+                ce.dequeue(this, e)
             })
         },
         clearQueue: function(e) {
             return this.queue(e || "fx", [])
         },
         promise: function(e, t) {
             var n, r = 1,
-                i = k.Deferred(),
+                i = ce.Deferred(),
                 o = this,
                 a = this.length,
                 s = function() {
                     --r || i.resolveWith(o, [o])
                 };
             "string" != typeof e && (t = e, e = void 0), e = e || "fx";
-            while (a--)(n = Q.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
+            while (a--)(n = _.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
             return s(), i.promise(t)
         }
     });
-    var te = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-        ne = new RegExp("^(?:([+-])=|)(" + te + ")([a-z%]*)$", "i"),
-        re = ["Top", "Right", "Bottom", "Left"],
-        ie = E.documentElement,
-        oe = function(e) {
-            return k.contains(e.ownerDocument, e)
+    var G = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        Y = new RegExp("^(?:([+-])=|)(" + G + ")([a-z%]*)$", "i"),
+        Q = ["Top", "Right", "Bottom", "Left"],
+        J = C.documentElement,
+        K = function(e) {
+            return ce.contains(e.ownerDocument, e)
         },
-        ae = {
+        Z = {
             composed: !0
         };
-    ie.getRootNode && (oe = function(e) {
-        return k.contains(e.ownerDocument, e) || e.getRootNode(ae) === e.ownerDocument
+    J.getRootNode && (K = function(e) {
+        return ce.contains(e.ownerDocument, e) || e.getRootNode(Z) === e.ownerDocument
     });
-    var se = function(e, t) {
-            return "none" === (e = t || e).style.display || "" === e.style.display && oe(e) && "none" === k.css(e, "display")
-        },
-        ue = function(e, t, n, r) {
-            var i, o, a = {};
-            for (o in t) a[o] = e.style[o], e.style[o] = t[o];
-            for (o in i = n.apply(e, r || []), t) e.style[o] = a[o];
-            return i
-        };
+    var ee = function(e, t) {
+        return "none" === (e = t || e).style.display || "" === e.style.display && K(e) && "none" === ce.css(e, "display")
+    };
 
-    function le(e, t, n, r) {
+    function te(e, t, n, r) {
         var i, o, a = 20,
             s = r ? function() {
                 return r.cur()
             } : function() {
-                return k.css(e, t, "")
+                return ce.css(e, t, "")
             },
             u = s(),
-            l = n && n[3] || (k.cssNumber[t] ? "" : "px"),
-            c = e.nodeType && (k.cssNumber[t] || "px" !== l && +u) && ne.exec(k.css(e, t));
+            l = n && n[3] || (ce.cssNumber[t] ? "" : "px"),
+            c = e.nodeType && (ce.cssNumber[t] || "px" !== l && +u) && Y.exec(ce.css(e, t));
         if (c && c[3] !== l) {
             u /= 2, l = l || c[3], c = +u || 1;
-            while (a--) k.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
-            c *= 2, k.style(e, t, c + l), n = n || []
+            while (a--) ce.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
+            c *= 2, ce.style(e, t, c + l), n = n || []
         }
         return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
     }
-    var ce = {};
+    var ne = {};
 
-    function fe(e, t) {
-        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = Q.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && se(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ce[s]) || (o = a.body.appendChild(a.createElement(s)), u = k.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ce[s] = u)))) : "none" !== n && (l[c] = "none", Q.set(r, "display", n)));
+    function re(e, t) {
+        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = _.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && ee(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ne[s]) || (o = a.body.appendChild(a.createElement(s)), u = ce.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ne[s] = u)))) : "none" !== n && (l[c] = "none", _.set(r, "display", n)));
         for (c = 0; c < f; c++) null != l[c] && (e[c].style.display = l[c]);
         return e
     }
-    k.fn.extend({
+    ce.fn.extend({
         show: function() {
-            return fe(this, !0)
+            return re(this, !0)
         },
         hide: function() {
-            return fe(this)
+            return re(this)
         },
         toggle: function(e) {
             return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each(function() {
-                se(this) ? k(this).show() : k(this).hide()
+                ee(this) ? ce(this).show() : ce(this).hide()
             })
         }
     });
-    var pe = /^(?:checkbox|radio)$/i,
-        de = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-        he = /^$|^module$|\/(?:java|ecma)script/i,
-        ge = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            thead: [1, "<table>", "</table>"],
-            col: [2, "<table><colgroup>", "</colgroup></table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            _default: [0, "", ""]
-        };
+    var xe, be, we = /^(?:checkbox|radio)$/i,
+        Te = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+        Ce = /^$|^module$|\/(?:java|ecma)script/i;
+    xe = C.createDocumentFragment().appendChild(C.createElement("div")), (be = C.createElement("input")).setAttribute("type", "radio"), be.setAttribute("checked", "checked"), be.setAttribute("name", "t"), xe.appendChild(be), le.checkClone = xe.cloneNode(!0).cloneNode(!0).lastChild.checked, xe.innerHTML = "<textarea>x</textarea>", le.noCloneChecked = !!xe.cloneNode(!0).lastChild.defaultValue, xe.innerHTML = "<option></option>", le.option = !!xe.lastChild;
+    var ke = {
+        thead: [1, "<table>", "</table>"],
+        col: [2, "<table><colgroup>", "</colgroup></table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+        _default: [0, "", ""]
+    };
 
-    function ve(e, t) {
+    function Se(e, t) {
         var n;
-        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && A(e, t) ? k.merge([e], n) : n
+        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && fe(e, t) ? ce.merge([e], n) : n
     }
 
-    function ye(e, t) {
-        for (var n = 0, r = e.length; n < r; n++) Q.set(e[n], "globalEval", !t || Q.get(t[n], "globalEval"))
+    function Ee(e, t) {
+        for (var n = 0, r = e.length; n < r; n++) _.set(e[n], "globalEval", !t || _.get(t[n], "globalEval"))
     }
-    ge.optgroup = ge.option, ge.tbody = ge.tfoot = ge.colgroup = ge.caption = ge.thead, ge.th = ge.td;
-    var me, xe, be = /<|&#?\w+;/;
+    ke.tbody = ke.tfoot = ke.colgroup = ke.caption = ke.thead, ke.th = ke.td, le.option || (ke.optgroup = ke.option = [1, "<select multiple='multiple'>", "</select>"]);
+    var je = /<|&#?\w+;/;
 
-    function we(e, t, n, r, i) {
+    function Ae(e, t, n, r, i) {
         for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
             if ((o = e[d]) || 0 === o)
-                if ("object" === w(o)) k.merge(p, o.nodeType ? [o] : o);
-                else if (be.test(o)) {
-            a = a || f.appendChild(t.createElement("div")), s = (de.exec(o) || ["", ""])[1].toLowerCase(), u = ge[s] || ge._default, a.innerHTML = u[1] + k.htmlPrefilter(o) + u[2], c = u[0];
+                if ("object" === x(o)) ce.merge(p, o.nodeType ? [o] : o);
+                else if (je.test(o)) {
+            a = a || f.appendChild(t.createElement("div")), s = (Te.exec(o) || ["", ""])[1].toLowerCase(), u = ke[s] || ke._default, a.innerHTML = u[1] + ce.htmlPrefilter(o) + u[2], c = u[0];
             while (c--) a = a.lastChild;
-            k.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
+            ce.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
         } else p.push(t.createTextNode(o));
         f.textContent = "", d = 0;
         while (o = p[d++])
-            if (r && -1 < k.inArray(o, r)) i && i.push(o);
-            else if (l = oe(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
+            if (r && -1 < ce.inArray(o, r)) i && i.push(o);
+            else if (l = K(o), a = Se(f.appendChild(o), "script"), l && Ee(a), n) {
             c = 0;
-            while (o = a[c++]) he.test(o.type || "") && n.push(o)
+            while (o = a[c++]) Ce.test(o.type || "") && n.push(o)
         }
         return f
     }
-    me = E.createDocumentFragment().appendChild(E.createElement("div")), (xe = E.createElement("input")).setAttribute("type", "radio"), xe.setAttribute("checked", "checked"), xe.setAttribute("name", "t"), me.appendChild(xe), y.checkClone = me.cloneNode(!0).cloneNode(!0).lastChild.checked, me.innerHTML = "<textarea>x</textarea>", y.noCloneChecked = !!me.cloneNode(!0).lastChild.defaultValue;
-    var Te = /^key/,
-        Ce = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Ee = /^([^.]*)(?:\.(.+)|)/;
+    var De = /^([^.]*)(?:\.(.+)|)/;
 
-    function ke() {
+    function Ne() {
         return !0
     }
 
-    function Se() {
+    function qe() {
         return !1
     }
 
-    function Ne(e, t) {
-        return e === function() {
-            try {
-                return E.activeElement
-            } catch (e) {}
-        }() == ("focus" === t)
-    }
-
-    function Ae(e, t, n, r, i, o) {
+    function Le(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ae(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Le(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Se;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = qe;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
-            return k().off(e), a.apply(this, arguments)
-        }).guid = a.guid || (a.guid = k.guid++)), e.each(function() {
-            k.event.add(this, t, i, r, n)
+            return ce().off(e), a.apply(this, arguments)
+        }).guid = a.guid || (a.guid = ce.guid++)), e.each(function() {
+            ce.event.add(this, t, i, r, n)
         })
     }
 
-    function De(e, i, o) {
-        o ? (Q.set(e, i, !1), k.event.add(e, i, {
+    function He(e, r, t) {
+        t ? (_.set(e, r, !1), ce.event.add(e, r, {
             namespace: !1,
             handler: function(e) {
-                var t, n, r = Q.get(this, i);
-                if (1 & e.isTrigger && this[i]) {
-                    if (r.length)(k.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Q.set(this, i, r), t = o(this, i), this[i](), r !== (n = Q.get(this, i)) || t ? Q.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
-                } else r.length && (Q.set(this, i, {
-                    value: k.event.trigger(k.extend(r[0], k.Event.prototype), r.slice(1), this)
-                }), e.stopImmediatePropagation())
+                var t, n = _.get(this, r);
+                if (1 & e.isTrigger && this[r]) {
+                    if (n)(ce.event.special[r] || {}).delegateType && e.stopPropagation();
+                    else if (n = ae.call(arguments), _.set(this, r, n), this[r](), t = _.get(this, r), _.set(this, r, !1), n !== t) return e.stopImmediatePropagation(), e.preventDefault(), t
+                } else n && (_.set(this, r, ce.event.trigger(n[0], n.slice(1), this)), e.stopPropagation(), e.isImmediatePropagationStopped = Ne)
             }
-        })) : void 0 === Q.get(e, i) && k.event.add(e, i, ke)
+        })) : void 0 === _.get(e, r) && ce.event.add(e, r, Ne)
     }
-    k.event = {
+    ce.event = {
         global: {},
         add: function(t, e, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.get(t);
-            if (v) {
-                n.handler && (n = (o = n).handler, i = o.selector), i && k.find.matchesSelector(ie, i), n.guid || (n.guid = k.guid++), (u = v.events) || (u = v.events = {}), (a = v.handle) || (a = v.handle = function(e) {
-                    return "undefined" != typeof k && k.event.triggered !== e.type ? k.event.dispatch.apply(t, arguments) : void 0
-                }), l = (e = (e || "").match(R) || [""]).length;
-                while (l--) d = g = (s = Ee.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = k.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = k.event.special[d] || {}, c = k.extend({
+            var o, a, s, u, l, c, f, p, d, h, g, v = _.get(t);
+            if ($(t)) {
+                n.handler && (n = (o = n).handler, i = o.selector), i && ce.find.matchesSelector(J, i), n.guid || (n.guid = ce.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
+                    return "undefined" != typeof ce && ce.event.triggered !== e.type ? ce.event.dispatch.apply(t, arguments) : void 0
+                }), l = (e = (e || "").match(D) || [""]).length;
+                while (l--) d = g = (s = De.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = ce.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = ce.event.special[d] || {}, c = ce.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
-                    needsContext: i && k.expr.match.needsContext.test(i),
+                    needsContext: i && ce.expr.match.needsContext.test(i),
                     namespace: h.join(".")
-                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), k.event.global[d] = !0)
+                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), ce.event.global[d] = !0)
             }
         },
         remove: function(e, t, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.hasData(e) && Q.get(e);
+            var o, a, s, u, l, c, f, p, d, h, g, v = _.hasData(e) && _.get(e);
             if (v && (u = v.events)) {
-                l = (t = (t || "").match(R) || [""]).length;
+                l = (t = (t || "").match(D) || [""]).length;
                 while (l--)
-                    if (d = g = (s = Ee.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
-                        f = k.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
+                    if (d = g = (s = De.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                        f = ce.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
-                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || k.removeEvent(e, d, v.handle), delete u[d])
+                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || ce.removeEvent(e, d, v.handle), delete u[d])
                     } else
-                        for (d in u) k.event.remove(e, d + t[l], n, r, !0);
-                k.isEmptyObject(u) && Q.remove(e, "handle events")
+                        for (d in u) ce.event.remove(e, d + t[l], n, r, !0);
+                ce.isEmptyObject(u) && _.remove(e, "handle events")
             }
         },
         dispatch: function(e) {
-            var t, n, r, i, o, a, s = k.event.fix(e),
-                u = new Array(arguments.length),
-                l = (Q.get(this, "events") || {})[s.type] || [],
-                c = k.event.special[s.type] || {};
-            for (u[0] = s, t = 1; t < arguments.length; t++) u[t] = arguments[t];
-            if (s.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, s)) {
-                a = k.event.handlers.call(this, s, l), t = 0;
-                while ((i = a[t++]) && !s.isPropagationStopped()) {
-                    s.currentTarget = i.elem, n = 0;
-                    while ((o = i.handlers[n++]) && !s.isImmediatePropagationStopped()) s.rnamespace && !1 !== o.namespace && !s.rnamespace.test(o.namespace) || (s.handleObj = o, s.data = o.data, void 0 !== (r = ((k.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, u)) && !1 === (s.result = r) && (s.preventDefault(), s.stopPropagation()))
+            var t, n, r, i, o, a, s = new Array(arguments.length),
+                u = ce.event.fix(e),
+                l = (_.get(this, "events") || Object.create(null))[u.type] || [],
+                c = ce.event.special[u.type] || {};
+            for (s[0] = u, t = 1; t < arguments.length; t++) s[t] = arguments[t];
+            if (u.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, u)) {
+                a = ce.event.handlers.call(this, u, l), t = 0;
+                while ((i = a[t++]) && !u.isPropagationStopped()) {
+                    u.currentTarget = i.elem, n = 0;
+                    while ((o = i.handlers[n++]) && !u.isImmediatePropagationStopped()) u.rnamespace && !1 !== o.namespace && !u.rnamespace.test(o.namespace) || (u.handleObj = o, u.data = o.data, void 0 !== (r = ((ce.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, s)) && !1 === (u.result = r) && (u.preventDefault(), u.stopPropagation()))
                 }
-                return c.postDispatch && c.postDispatch.call(this, s), s.result
+                return c.postDispatch && c.postDispatch.call(this, u), u.result
             }
         },
         handlers: function(e, t) {
             var n, r, i, o, a, s = [],
                 u = t.delegateCount,
                 l = e.target;
             if (u && l.nodeType && !("click" === e.type && 1 <= e.button))
                 for (; l !== this; l = l.parentNode || this)
                     if (1 === l.nodeType && ("click" !== e.type || !0 !== l.disabled)) {
-                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < k(i, this).index(l) : k.find(i, this, null, [l]).length), a[i] && o.push(r);
+                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < ce(i, this).index(l) : ce.find(i, this, null, [l]).length), a[i] && o.push(r);
                         o.length && s.push({
                             elem: l,
                             handlers: o
                         })
                     } return l = this, u < t.length && s.push({
                 elem: l,
                 handlers: t.slice(u)
             }), s
         },
         addProp: function(t, e) {
-            Object.defineProperty(k.Event.prototype, t, {
+            Object.defineProperty(ce.Event.prototype, t, {
                 enumerable: !0,
                 configurable: !0,
-                get: m(e) ? function() {
+                get: v(e) ? function() {
                     if (this.originalEvent) return e(this.originalEvent)
                 } : function() {
                     if (this.originalEvent) return this.originalEvent[t]
                 },
                 set: function(e) {
                     Object.defineProperty(this, t, {
                         enumerable: !0,
@@ -1643,64 +1580,64 @@
                         writable: !0,
                         value: e
                     })
                 }
             })
         },
         fix: function(e) {
-            return e[k.expando] ? e : new k.Event(e)
+            return e[ce.expando] ? e : new ce.Event(e)
         },
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click", ke), !1
+                    return we.test(t.type) && t.click && fe(t, "input") && He(t, "click", !0), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click"), !0
+                    return we.test(t.type) && t.click && fe(t, "input") && He(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
-                    return pe.test(t.type) && t.click && A(t, "input") && Q.get(t, "click") || A(t, "a")
+                    return we.test(t.type) && t.click && fe(t, "input") && _.get(t, "click") || fe(t, "a")
                 }
             },
             beforeunload: {
                 postDispatch: function(e) {
                     void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
                 }
             }
         }
-    }, k.removeEvent = function(e, t, n) {
+    }, ce.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
-    }, k.Event = function(e, t) {
-        if (!(this instanceof k.Event)) return new k.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? ke : Se, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && k.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[k.expando] = !0
-    }, k.Event.prototype = {
-        constructor: k.Event,
-        isDefaultPrevented: Se,
-        isPropagationStopped: Se,
-        isImmediatePropagationStopped: Se,
+    }, ce.Event = function(e, t) {
+        if (!(this instanceof ce.Event)) return new ce.Event(e, t);
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ne : qe, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && ce.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[ce.expando] = !0
+    }, ce.Event.prototype = {
+        constructor: ce.Event,
+        isDefaultPrevented: qe,
+        isPropagationStopped: qe,
+        isImmediatePropagationStopped: qe,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = ke, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = Ne, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = ke, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = Ne, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = ke, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = Ne, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
-    }, k.each({
+    }, ce.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
         detail: !0,
         eventPhase: !0,
@@ -1723,1045 +1660,1068 @@
         pointerId: !0,
         pointerType: !0,
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
-        which: function(e) {
-            var t = e.button;
-            return null == e.which && Te.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && Ce.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
-        }
-    }, k.event.addProp), k.each({
+        which: !0
+    }, ce.event.addProp), ce.each({
         focus: "focusin",
         blur: "focusout"
-    }, function(e, t) {
-        k.event.special[e] = {
+    }, function(r, i) {
+        function o(e) {
+            if (C.documentMode) {
+                var t = _.get(this, "handle"),
+                    n = ce.event.fix(e);
+                n.type = "focusin" === e.type ? "focus" : "blur", n.isSimulated = !0, t(e), n.target === n.currentTarget && t(n)
+            } else ce.event.simulate(i, e.target, ce.event.fix(e))
+        }
+        ce.event.special[r] = {
             setup: function() {
-                return De(this, e, Ne), !1
+                var e;
+                if (He(this, r, !0), !C.documentMode) return !1;
+                (e = _.get(this, i)) || this.addEventListener(i, o), _.set(this, i, (e || 0) + 1)
             },
             trigger: function() {
-                return De(this, e), !0
+                return He(this, r), !0
             },
-            delegateType: t
+            teardown: function() {
+                var e;
+                if (!C.documentMode) return !1;
+                (e = _.get(this, i) - 1) ? _.set(this, i, e): (this.removeEventListener(i, o), _.remove(this, i))
+            },
+            _default: function(e) {
+                return _.get(e.target, r)
+            },
+            delegateType: i
+        }, ce.event.special[i] = {
+            setup: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = C.documentMode ? this : e,
+                    n = _.get(t, i);
+                n || (C.documentMode ? this.addEventListener(i, o) : e.addEventListener(r, o, !0)), _.set(t, i, (n || 0) + 1)
+            },
+            teardown: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = C.documentMode ? this : e,
+                    n = _.get(t, i) - 1;
+                n ? _.set(t, i, n) : (C.documentMode ? this.removeEventListener(i, o) : e.removeEventListener(r, o, !0), _.remove(t, i))
+            }
         }
-    }), k.each({
+    }), ce.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
         pointerleave: "pointerout"
     }, function(e, i) {
-        k.event.special[e] = {
+        ce.event.special[e] = {
             delegateType: i,
             bindType: i,
             handle: function(e) {
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
-                return n && (n === this || k.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
+                return n && (n === this || ce.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         on: function(e, t, n, r) {
-            return Ae(this, e, t, n, r)
+            return Le(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return Ae(this, e, t, n, r, 1)
+            return Le(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
-            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, k(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
+            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, ce(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Se), this.each(function() {
-                k.event.remove(this, e, n, t)
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = qe), this.each(function() {
+                ce.event.remove(this, e, n, t)
             })
         }
     });
-    var je = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,
-        qe = /<script|<style|<link/i,
-        Le = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        He = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var Oe = /<script|<style|<link/i,
+        Pe = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Re = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
-    function Oe(e, t) {
-        return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && k(e).children("tbody")[0] || e
+    function Me(e, t) {
+        return fe(e, "table") && fe(11 !== t.nodeType ? t : t.firstChild, "tr") && ce(e).children("tbody")[0] || e
     }
 
-    function Pe(e) {
+    function Ie(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function Re(e) {
+    function We(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Me(e, t) {
-        var n, r, i, o, a, s, u, l;
+    function Fe(e, t) {
+        var n, r, i, o, a, s;
         if (1 === t.nodeType) {
-            if (Q.hasData(e) && (o = Q.access(e), a = Q.set(t, o), l = o.events))
-                for (i in delete a.handle, a.events = {}, l)
-                    for (n = 0, r = l[i].length; n < r; n++) k.event.add(t, i, l[i][n]);
-            J.hasData(e) && (s = J.access(e), u = k.extend({}, s), J.set(t, u))
+            if (_.hasData(e) && (s = _.get(e).events))
+                for (i in _.remove(t, "handle events"), s)
+                    for (n = 0, r = s[i].length; n < r; n++) ce.event.add(t, i, s[i][n]);
+            X.hasData(e) && (o = X.access(e), a = ce.extend({}, o), X.set(t, a))
         }
     }
 
-    function Ie(n, r, i, o) {
-        r = g.apply([], r);
+    function $e(n, r, i, o) {
+        r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
-            h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && Le.test(d)) return n.each(function(e) {
+            h = v(d);
+        if (h || 1 < f && "string" == typeof d && !le.checkClone && Pe.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Ie(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), $e(t, r, i, o)
         });
-        if (f && (t = (e = we(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = k.map(ve(e, "script"), Pe)).length; c < f; c++) u = e, c !== p && (u = k.clone(u, !0, !0), s && k.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+        if (f && (t = (e = Ae(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
+            for (s = (a = ce.map(Se(e, "script"), Ie)).length; c < f; c++) u = e, c !== p && (u = ce.clone(u, !0, !0), s && ce.merge(a, Se(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, k.map(a, Re), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Q.access(u, "globalEval") && k.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? k._evalUrl && !u.noModule && k._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, ce.map(a, We), c = 0; c < s; c++) u = a[c], Ce.test(u.type || "") && !_.access(u, "globalEval") && ce.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? ce._evalUrl && !u.noModule && ce._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }) : b(u.textContent.replace(He, ""), u, l))
+                }, l) : m(u.textContent.replace(Re, ""), u, l))
         }
         return n
     }
 
-    function We(e, t, n) {
-        for (var r, i = t ? k.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || k.cleanData(ve(r)), r.parentNode && (n && oe(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
+    function Be(e, t, n) {
+        for (var r, i = t ? ce.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || ce.cleanData(Se(r)), r.parentNode && (n && K(r) && Ee(Se(r, "script")), r.parentNode.removeChild(r));
         return e
     }
-    k.extend({
+    ce.extend({
         htmlPrefilter: function(e) {
-            return e.replace(je, "<$1></$2>")
+            return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
-                f = oe(e);
-            if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || k.isXMLDoc(e)))
-                for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
+                f = K(e);
+            if (!(le.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || ce.isXMLDoc(e)))
+                for (a = Se(c), r = 0, i = (o = Se(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && we.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Me(o[r], a[r]);
-                else Me(e, c);
-            return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
+                    for (o = o || Se(e), a = a || Se(c), r = 0, i = o.length; r < i; r++) Fe(o[r], a[r]);
+                else Fe(e, c);
+            return 0 < (a = Se(c, "script")).length && Ee(a, !f && Se(e, "script")), c
         },
         cleanData: function(e) {
-            for (var t, n, r, i = k.event.special, o = 0; void 0 !== (n = e[o]); o++)
-                if (G(n)) {
-                    if (t = n[Q.expando]) {
+            for (var t, n, r, i = ce.event.special, o = 0; void 0 !== (n = e[o]); o++)
+                if ($(n)) {
+                    if (t = n[_.expando]) {
                         if (t.events)
-                            for (r in t.events) i[r] ? k.event.remove(n, r) : k.removeEvent(n, r, t.handle);
-                        n[Q.expando] = void 0
+                            for (r in t.events) i[r] ? ce.event.remove(n, r) : ce.removeEvent(n, r, t.handle);
+                        n[_.expando] = void 0
                     }
-                    n[J.expando] && (n[J.expando] = void 0)
+                    n[X.expando] && (n[X.expando] = void 0)
                 }
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         detach: function(e) {
-            return We(this, e, !0)
+            return Be(this, e, !0)
         },
         remove: function(e) {
-            return We(this, e)
+            return Be(this, e)
         },
         text: function(e) {
-            return _(this, function(e) {
-                return void 0 === e ? k.text(this) : this.empty().each(function() {
+            return R(this, function(e) {
+                return void 0 === e ? ce.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return Ie(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || Oe(this, e).appendChild(e)
+            return $e(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || Me(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return Ie(this, arguments, function(e) {
+            return $e(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = Oe(this, e);
+                    var t = Me(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return Ie(this, arguments, function(e) {
+            return $e(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return Ie(this, arguments, function(e) {
+            return $e(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
-            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (k.cleanData(ve(e, !1)), e.textContent = "");
+            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (ce.cleanData(Se(e, !1)), e.textContent = "");
             return this
         },
         clone: function(e, t) {
             return e = null != e && e, t = null == t ? e : t, this.map(function() {
-                return k.clone(this, e, t)
+                return ce.clone(this, e, t)
             })
         },
         html: function(e) {
-            return _(this, function(e) {
+            return R(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !qe.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
-                    e = k.htmlPrefilter(e);
+                if ("string" == typeof e && !Oe.test(e) && !ke[(Te.exec(e) || ["", ""])[1].toLowerCase()]) {
+                    e = ce.htmlPrefilter(e);
                     try {
-                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (k.cleanData(ve(t, !1)), t.innerHTML = e);
+                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (ce.cleanData(Se(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return Ie(this, arguments, function(e) {
+            return $e(this, arguments, function(e) {
                 var t = this.parentNode;
-                k.inArray(this, n) < 0 && (k.cleanData(ve(this)), t && t.replaceChild(e, this))
+                ce.inArray(this, n) < 0 && (ce.cleanData(Se(this)), t && t.replaceChild(e, this))
             }, n)
         }
-    }), k.each({
+    }), ce.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
     }, function(e, a) {
-        k.fn[e] = function(e) {
-            for (var t, n = [], r = k(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), k(r[o])[a](t), u.apply(n, t.get());
+        ce.fn[e] = function(e) {
+            for (var t, n = [], r = ce(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), ce(r[o])[a](t), s.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var $e = new RegExp("^(" + te + ")(?!px)[a-z%]+$", "i"),
-        Fe = function(e) {
+    var _e = new RegExp("^(" + G + ")(?!px)[a-z%]+$", "i"),
+        Xe = /^--/,
+        Ue = function(e) {
             var t = e.ownerDocument.defaultView;
-            return t && t.opener || (t = C), t.getComputedStyle(e)
+            return t && t.opener || (t = ie), t.getComputedStyle(e)
+        },
+        ze = function(e, t, n) {
+            var r, i, o = {};
+            for (i in t) o[i] = e.style[i], e.style[i] = t[i];
+            for (i in r = n.call(e), t) e.style[i] = o[i];
+            return r
         },
-        Be = new RegExp(re.join("|"), "i");
+        Ve = new RegExp(Q.join("|"), "i");
 
-    function _e(e, t, n) {
-        var r, i, o, a, s = e.style;
-        return (n = n || Fe(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || oe(e) || (a = k.style(e, t)), !y.pixelBoxStyles() && $e.test(a) && Be.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+    function Ge(e, t, n) {
+        var r, i, o, a, s = Xe.test(t),
+            u = e.style;
+        return (n = n || Ue(e)) && (a = n.getPropertyValue(t) || n[t], s && a && (a = a.replace(ve, "$1") || void 0), "" !== a || K(e) || (a = ce.style(e, t)), !le.pixelBoxStyles() && _e.test(a) && Ve.test(t) && (r = u.width, i = u.minWidth, o = u.maxWidth, u.minWidth = u.maxWidth = u.width = a, a = n.width, u.width = r, u.minWidth = i, u.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function ze(e, t) {
+    function Ye(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
         function e() {
-            if (u) {
-                s.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", u.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ie.appendChild(s).appendChild(u);
-                var e = C.getComputedStyle(u);
-                n = "1%" !== e.top, a = 12 === t(e.marginLeft), u.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), u.style.position = "absolute", i = 12 === t(u.offsetWidth / 3), ie.removeChild(s), u = null
+            if (l) {
+                u.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", l.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", J.appendChild(u).appendChild(l);
+                var e = ie.getComputedStyle(l);
+                n = "1%" !== e.top, s = 12 === t(e.marginLeft), l.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), l.style.position = "absolute", i = 12 === t(l.offsetWidth / 3), J.removeChild(u), l = null
             }
         }
 
         function t(e) {
             return Math.round(parseFloat(e))
         }
-        var n, r, i, o, a, s = E.createElement("div"),
-            u = E.createElement("div");
-        u.style && (u.style.backgroundClip = "content-box", u.cloneNode(!0).style.backgroundClip = "", y.clearCloneStyle = "content-box" === u.style.backgroundClip, k.extend(y, {
+        var n, r, i, o, a, s, u = C.createElement("div"),
+            l = C.createElement("div");
+        l.style && (l.style.backgroundClip = "content-box", l.cloneNode(!0).style.backgroundClip = "", le.clearCloneStyle = "content-box" === l.style.backgroundClip, ce.extend(le, {
             boxSizingReliable: function() {
                 return e(), r
             },
             pixelBoxStyles: function() {
                 return e(), o
             },
             pixelPosition: function() {
                 return e(), n
             },
             reliableMarginLeft: function() {
-                return e(), a
+                return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
+            },
+            reliableTrDimensions: function() {
+                var e, t, n, r;
+                return null == a && (e = C.createElement("table"), t = C.createElement("tr"), n = C.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", J.appendChild(e).appendChild(t).appendChild(n), r = ie.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, J.removeChild(e)), a
             }
         }))
     }();
-    var Ue = ["Webkit", "Moz", "ms"],
-        Xe = E.createElement("div").style,
-        Ve = {};
-
-    function Ge(e) {
-        var t = k.cssProps[e] || Ve[e];
-        return t || (e in Xe ? e : Ve[e] = function(e) {
+    var Qe = ["Webkit", "Moz", "ms"],
+        Je = C.createElement("div").style,
+        Ke = {};
+
+    function Ze(e) {
+        var t = ce.cssProps[e] || Ke[e];
+        return t || (e in Je ? e : Ke[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = Ue.length;
+                n = Qe.length;
             while (n--)
-                if ((e = Ue[n] + t) in Xe) return e
+                if ((e = Qe[n] + t) in Je) return e
         }(e) || e)
     }
-    var Ye = /^(none|table(?!-c[ea]).+)/,
-        Qe = /^--/,
-        Je = {
+    var et = /^(none|table(?!-c[ea]).+)/,
+        tt = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Ke = {
+        nt = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Ze(e, t, n) {
-        var r = ne.exec(t);
+    function rt(e, t, n) {
+        var r = Y.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function et(e, t, n, r, i, o) {
+    function it(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
-            u = 0;
+            u = 0,
+            l = 0;
         if (n === (r ? "border" : "content")) return 0;
-        for (; a < 4; a += 2) "margin" === n && (u += k.css(e, n + re[a], !0, i)), r ? ("content" === n && (u -= k.css(e, "padding" + re[a], !0, i)), "margin" !== n && (u -= k.css(e, "border" + re[a] + "Width", !0, i))) : (u += k.css(e, "padding" + re[a], !0, i), "padding" !== n ? u += k.css(e, "border" + re[a] + "Width", !0, i) : s += k.css(e, "border" + re[a] + "Width", !0, i));
-        return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
+        for (; a < 4; a += 2) "margin" === n && (l += ce.css(e, n + Q[a], !0, i)), r ? ("content" === n && (u -= ce.css(e, "padding" + Q[a], !0, i)), "margin" !== n && (u -= ce.css(e, "border" + Q[a] + "Width", !0, i))) : (u += ce.css(e, "padding" + Q[a], !0, i), "padding" !== n ? u += ce.css(e, "border" + Q[a] + "Width", !0, i) : s += ce.css(e, "border" + Q[a] + "Width", !0, i));
+        return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u + l
     }
 
-    function tt(e, t, n) {
-        var r = Fe(e),
-            i = (!y.boxSizingReliable() || n) && "border-box" === k.css(e, "boxSizing", !1, r),
+    function ot(e, t, n) {
+        var r = Ue(e),
+            i = (!le.boxSizingReliable() || n) && "border-box" === ce.css(e, "boxSizing", !1, r),
             o = i,
-            a = _e(e, t, r),
+            a = Ge(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if ($e.test(a)) {
+        if (_e.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || "auto" === a || !parseFloat(a) && "inline" === k.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === k.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + et(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!le.boxSizingReliable() && i || !le.reliableTrDimensions() && fe(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === ce.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === ce.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + it(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function nt(e, t, n, r, i) {
-        return new nt.prototype.init(e, t, n, r, i)
+    function at(e, t, n, r, i) {
+        return new at.prototype.init(e, t, n, r, i)
     }
-    k.extend({
+    ce.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = _e(e, "opacity");
+                        var n = Ge(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
+            aspectRatio: !0,
+            borderImageSlice: !0,
             columnCount: !0,
-            fillOpacity: !0,
             flexGrow: !0,
             flexShrink: !0,
             fontWeight: !0,
             gridArea: !0,
             gridColumn: !0,
             gridColumnEnd: !0,
             gridColumnStart: !0,
             gridRow: !0,
             gridRowEnd: !0,
             gridRowStart: !0,
             lineHeight: !0,
             opacity: !0,
             order: !0,
             orphans: !0,
+            scale: !0,
             widows: !0,
             zIndex: !0,
-            zoom: !0
+            zoom: !0,
+            fillOpacity: !0,
+            floodOpacity: !0,
+            stopOpacity: !0,
+            strokeMiterlimit: !0,
+            strokeOpacity: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
-                var i, o, a, s = V(t),
-                    u = Qe.test(t),
+                var i, o, a, s = F(t),
+                    u = Xe.test(t),
                     l = e.style;
-                if (u || (t = Ge(s)), a = k.cssHooks[t] || k.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
-                "string" === (o = typeof n) && (i = ne.exec(n)) && i[1] && (n = le(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (k.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
+                if (u || (t = Ze(s)), a = ce.cssHooks[t] || ce.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                "string" === (o = typeof n) && (i = Y.exec(n)) && i[1] && (n = te(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (ce.cssNumber[s] ? "" : "px")), le.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
-            var i, o, a, s = V(t);
-            return Qe.test(t) || (t = Ge(s)), (a = k.cssHooks[t] || k.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = _e(e, t, r)), "normal" === i && t in Ke && (i = Ke[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            var i, o, a, s = F(t);
+            return Xe.test(t) || (t = Ze(s)), (a = ce.cssHooks[t] || ce.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Ge(e, t, r)), "normal" === i && t in nt && (i = nt[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
-    }), k.each(["height", "width"], function(e, u) {
-        k.cssHooks[u] = {
+    }), ce.each(["height", "width"], function(e, u) {
+        ce.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ye.test(k.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? tt(e, u, n) : ue(e, Je, function() {
-                    return tt(e, u, n)
+                if (t) return !et.test(ce.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? ot(e, u, n) : ze(e, tt, function() {
+                    return ot(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Fe(e),
-                    o = !y.scrollboxSize() && "absolute" === i.position,
-                    a = (o || n) && "border-box" === k.css(e, "boxSizing", !1, i),
-                    s = n ? et(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - et(e, u, "border", !1, i) - .5)), s && (r = ne.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = k.css(e, u)), Ze(0, t, s)
+                var r, i = Ue(e),
+                    o = !le.scrollboxSize() && "absolute" === i.position,
+                    a = (o || n) && "border-box" === ce.css(e, "boxSizing", !1, i),
+                    s = n ? it(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - it(e, u, "border", !1, i) - .5)), s && (r = Y.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = ce.css(e, u)), rt(0, t, s)
             }
         }
-    }), k.cssHooks.marginLeft = ze(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(_e(e, "marginLeft")) || e.getBoundingClientRect().left - ue(e, {
+    }), ce.cssHooks.marginLeft = Ye(le.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(Ge(e, "marginLeft")) || e.getBoundingClientRect().left - ze(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
-    }), k.each({
+    }), ce.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
-        k.cssHooks[i + o] = {
+        ce.cssHooks[i + o] = {
             expand: function(e) {
-                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + re[t] + o] = r[t] || r[t - 2] || r[0];
+                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + Q[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (k.cssHooks[i + o].set = Ze)
-    }), k.fn.extend({
+        }, "margin" !== i && (ce.cssHooks[i + o].set = rt)
+    }), ce.fn.extend({
         css: function(e, t) {
-            return _(this, function(e, t, n) {
+            return R(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Fe(e), i = t.length; a < i; a++) o[t[a]] = k.css(e, t[a], !1, r);
+                    for (r = Ue(e), i = t.length; a < i; a++) o[t[a]] = ce.css(e, t[a], !1, r);
                     return o
                 }
-                return void 0 !== n ? k.style(e, t, n) : k.css(e, t)
+                return void 0 !== n ? ce.style(e, t, n) : ce.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((k.Tween = nt).prototype = {
-        constructor: nt,
+    }), ((ce.Tween = at).prototype = {
+        constructor: at,
         init: function(e, t, n, r, i, o) {
-            this.elem = e, this.prop = n, this.easing = i || k.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (k.cssNumber[n] ? "" : "px")
+            this.elem = e, this.prop = n, this.easing = i || ce.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (ce.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = nt.propHooks[this.prop];
-            return e && e.get ? e.get(this) : nt.propHooks._default.get(this)
+            var e = at.propHooks[this.prop];
+            return e && e.get ? e.get(this) : at.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = nt.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = k.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : nt.propHooks._default.set(this), this
+            var t, n = at.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = ce.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : at.propHooks._default.set(this), this
         }
-    }).init.prototype = nt.prototype, (nt.propHooks = {
+    }).init.prototype = at.prototype, (at.propHooks = {
         _default: {
             get: function(e) {
                 var t;
-                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = k.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
+                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = ce.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                k.fx.step[e.prop] ? k.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !k.cssHooks[e.prop] && null == e.elem.style[Ge(e.prop)] ? e.elem[e.prop] = e.now : k.style(e.elem, e.prop, e.now + e.unit)
+                ce.fx.step[e.prop] ? ce.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !ce.cssHooks[e.prop] && null == e.elem.style[Ze(e.prop)] ? e.elem[e.prop] = e.now : ce.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = nt.propHooks.scrollLeft = {
+    }).scrollTop = at.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
-    }, k.easing = {
+    }, ce.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, k.fx = nt.prototype.init, k.fx.step = {};
-    var rt, it, ot, at, st = /^(?:toggle|show|hide)$/,
-        ut = /queueHooks$/;
+    }, ce.fx = at.prototype.init, ce.fx.step = {};
+    var st, ut, lt, ct, ft = /^(?:toggle|show|hide)$/,
+        pt = /queueHooks$/;
 
-    function lt() {
-        it && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(lt) : C.setTimeout(lt, k.fx.interval), k.fx.tick())
+    function dt() {
+        ut && (!1 === C.hidden && ie.requestAnimationFrame ? ie.requestAnimationFrame(dt) : ie.setTimeout(dt, ce.fx.interval), ce.fx.tick())
     }
 
-    function ct() {
-        return C.setTimeout(function() {
-            rt = void 0
-        }), rt = Date.now()
+    function ht() {
+        return ie.setTimeout(function() {
+            st = void 0
+        }), st = Date.now()
     }
 
-    function ft(e, t) {
+    function gt(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
-        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = re[r])] = i["padding" + n] = e;
+        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = Q[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function pt(e, t, n) {
-        for (var r, i = (dt.tweeners[t] || []).concat(dt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function vt(e, t, n) {
+        for (var r, i = (yt.tweeners[t] || []).concat(yt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function dt(o, e, t) {
+    function yt(o, e, t) {
         var n, a, r = 0,
-            i = dt.prefilters.length,
-            s = k.Deferred().always(function() {
+            i = yt.prefilters.length,
+            s = ce.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = rt || ct(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = st || ht(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
-                props: k.extend({}, e),
-                opts: k.extend(!0, {
+                props: ce.extend({}, e),
+                opts: ce.extend(!0, {
                     specialEasing: {},
-                    easing: k.easing._default
+                    easing: ce.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: rt || ct(),
+                startTime: st || ht(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
-                    var n = k.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
+                    var n = ce.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
                     var t = 0,
                         n = e ? l.tweens.length : 0;
                     if (a) return this;
                     for (a = !0; t < n; t++) l.tweens[t].run(1);
                     return e ? (s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l, e])) : s.rejectWith(o, [l, e]), this
                 }
             }),
             c = l.props;
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
-                    if (i = t[r = V(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = k.cssHooks[r]) && "expand" in a)
+                    if (i = t[r = F(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = ce.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = dt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (k._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return k.map(c, pt, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), k.fx.timer(k.extend(u, {
+            if (n = yt.prefilters[r].call(l, o, c, l.opts)) return v(n.stop) && (ce._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return ce.map(c, vt, l), v(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), ce.fx.timer(ce.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    k.Animation = k.extend(dt, {
+    ce.Animation = ce.extend(yt, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
-                return le(n.elem, e, ne.exec(t), n), n
+                return te(n.elem, e, Y.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
-            m(e) ? (t = e, e = ["*"]) : e = e.match(R);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], dt.tweeners[n] = dt.tweeners[n] || [], dt.tweeners[n].unshift(t)
+            v(e) ? (t = e, e = ["*"]) : e = e.match(D);
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], yt.tweeners[n] = yt.tweeners[n] || [], yt.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
-                g = e.nodeType && se(e),
-                v = Q.get(e, "fxshow");
-            for (r in n.queue || (null == (a = k._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
+                g = e.nodeType && ee(e),
+                v = _.get(e, "fxshow");
+            for (r in n.queue || (null == (a = ce._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
-                        a.unqueued--, k.queue(e, "fx").length || a.empty.fire()
+                        a.unqueued--, ce.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], st.test(i)) {
+                if (i = t[r], ft.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
-                    d[r] = v && v[r] || k.style(e, r)
-                } if ((u = !k.isEmptyObject(t)) || !k.isEmptyObject(d))
-                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Q.get(e, "display")), "none" === (c = k.css(e, "display")) && (l ? c = l : (fe([e], !0), l = e.style.display || l, c = k.css(e, "display"), fe([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === k.css(e, "float") && (u || (p.done(function() {
+                    d[r] = v && v[r] || ce.style(e, r)
+                } if ((u = !ce.isEmptyObject(t)) || !ce.isEmptyObject(d))
+                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = _.get(e, "display")), "none" === (c = ce.css(e, "display")) && (l ? c = l : (re([e], !0), l = e.style.display || l, c = ce.css(e, "display"), re([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === ce.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
-                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Q.access(e, "fxshow", {
+                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = _.access(e, "fxshow", {
                     display: l
-                }), o && (v.hidden = !g), g && fe([e], !0), p.done(function() {
-                    for (r in g || fe([e]), Q.remove(e, "fxshow"), d) k.style(e, r, d[r])
-                })), u = pt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                }), o && (v.hidden = !g), g && re([e], !0), p.done(function() {
+                    for (r in g || re([e]), _.remove(e, "fxshow"), d) ce.style(e, r, d[r])
+                })), u = vt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? dt.prefilters.unshift(e) : dt.prefilters.push(e)
+            t ? yt.prefilters.unshift(e) : yt.prefilters.push(e)
         }
-    }), k.speed = function(e, t, n) {
-        var r = e && "object" == typeof e ? k.extend({}, e) : {
-            complete: n || !n && t || m(e) && e,
+    }), ce.speed = function(e, t, n) {
+        var r = e && "object" == typeof e ? ce.extend({}, e) : {
+            complete: n || !n && t || v(e) && e,
             duration: e,
-            easing: n && t || t && !m(t) && t
+            easing: n && t || t && !v(t) && t
         };
-        return k.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in k.fx.speeds ? r.duration = k.fx.speeds[r.duration] : r.duration = k.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
-            m(r.old) && r.old.call(this), r.queue && k.dequeue(this, r.queue)
+        return ce.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in ce.fx.speeds ? r.duration = ce.fx.speeds[r.duration] : r.duration = ce.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
+            v(r.old) && r.old.call(this), r.queue && ce.dequeue(this, r.queue)
         }, r
-    }, k.fn.extend({
+    }, ce.fn.extend({
         fadeTo: function(e, t, n, r) {
-            return this.filter(se).css("opacity", 0).show().end().animate({
+            return this.filter(ee).css("opacity", 0).show().end().animate({
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
-            var i = k.isEmptyObject(t),
-                o = k.speed(e, n, r),
+            var i = ce.isEmptyObject(t),
+                o = ce.speed(e, n, r),
                 a = function() {
-                    var e = dt(this, k.extend({}, t), o);
-                    (i || Q.get(this, "finish")) && e.stop(!0)
+                    var e = yt(this, ce.extend({}, t), o);
+                    (i || _.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
                 delete e.stop, t(o)
             };
-            return "string" != typeof i && (o = e, e = i, i = void 0), e && !1 !== i && this.queue(i || "fx", []), this.each(function() {
+            return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
-                    n = k.timers,
-                    r = Q.get(this);
+                    n = ce.timers,
+                    r = _.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && ut.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && pt.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
-                !e && o || k.dequeue(this, i)
+                !e && o || ce.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
-                var e, t = Q.get(this),
+                var e, t = _.get(this),
                     n = t[a + "queue"],
                     r = t[a + "queueHooks"],
-                    i = k.timers,
+                    i = ce.timers,
                     o = n ? n.length : 0;
-                for (t.finish = !0, k.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
+                for (t.finish = !0, ce.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
-    }), k.each(["toggle", "show", "hide"], function(e, r) {
-        var i = k.fn[r];
-        k.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(ft(r, !0), e, t, n)
-        }
-    }), k.each({
-        slideDown: ft("show"),
-        slideUp: ft("hide"),
-        slideToggle: ft("toggle"),
+    }), ce.each(["toggle", "show", "hide"], function(e, r) {
+        var i = ce.fn[r];
+        ce.fn[r] = function(e, t, n) {
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(gt(r, !0), e, t, n)
+        }
+    }), ce.each({
+        slideDown: gt("show"),
+        slideUp: gt("hide"),
+        slideToggle: gt("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
             opacity: "toggle"
         }
     }, function(e, r) {
-        k.fn[e] = function(e, t, n) {
+        ce.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
-    }), k.timers = [], k.fx.tick = function() {
+    }), ce.timers = [], ce.fx.tick = function() {
         var e, t = 0,
-            n = k.timers;
-        for (rt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || k.fx.stop(), rt = void 0
-    }, k.fx.timer = function(e) {
-        k.timers.push(e), k.fx.start()
-    }, k.fx.interval = 13, k.fx.start = function() {
-        it || (it = !0, lt())
-    }, k.fx.stop = function() {
-        it = null
-    }, k.fx.speeds = {
+            n = ce.timers;
+        for (st = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || ce.fx.stop(), st = void 0
+    }, ce.fx.timer = function(e) {
+        ce.timers.push(e), ce.fx.start()
+    }, ce.fx.interval = 13, ce.fx.start = function() {
+        ut || (ut = !0, dt())
+    }, ce.fx.stop = function() {
+        ut = null
+    }, ce.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
-    }, k.fn.delay = function(r, e) {
-        return r = k.fx && k.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
-            var n = C.setTimeout(e, r);
+    }, ce.fn.delay = function(r, e) {
+        return r = ce.fx && ce.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
+            var n = ie.setTimeout(e, r);
             t.stop = function() {
-                C.clearTimeout(n)
+                ie.clearTimeout(n)
             }
         })
-    }, ot = E.createElement("input"), at = E.createElement("select").appendChild(E.createElement("option")), ot.type = "checkbox", y.checkOn = "" !== ot.value, y.optSelected = at.selected, (ot = E.createElement("input")).value = "t", ot.type = "radio", y.radioValue = "t" === ot.value;
-    var ht, gt = k.expr.attrHandle;
-    k.fn.extend({
+    }, lt = C.createElement("input"), ct = C.createElement("select").appendChild(C.createElement("option")), lt.type = "checkbox", le.checkOn = "" !== lt.value, le.optSelected = ct.selected, (lt = C.createElement("input")).value = "t", lt.type = "radio", le.radioValue = "t" === lt.value;
+    var mt, xt = ce.expr.attrHandle;
+    ce.fn.extend({
         attr: function(e, t) {
-            return _(this, k.attr, e, t, 1 < arguments.length)
+            return R(this, ce.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
-                k.removeAttr(this, e)
+                ce.removeAttr(this, e)
             })
         }
-    }), k.extend({
+    }), ce.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? k.prop(e, t, n) : (1 === o && k.isXMLDoc(e) || (i = k.attrHooks[t.toLowerCase()] || (k.expr.match.bool.test(t) ? ht : void 0)), void 0 !== n ? null === n ? void k.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = k.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? ce.prop(e, t, n) : (1 === o && ce.isXMLDoc(e) || (i = ce.attrHooks[t.toLowerCase()] || (ce.expr.match.bool.test(t) ? mt : void 0)), void 0 !== n ? null === n ? void ce.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = ce.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
-                    if (!y.radioValue && "radio" === t && A(e, "input")) {
+                    if (!le.radioValue && "radio" === t && fe(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
                     }
                 }
             }
         },
         removeAttr: function(e, t) {
             var n, r = 0,
-                i = t && t.match(R);
+                i = t && t.match(D);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), ht = {
+    }), mt = {
         set: function(e, t, n) {
-            return !1 === t ? k.removeAttr(e, n) : e.setAttribute(n, n), n
+            return !1 === t ? ce.removeAttr(e, n) : e.setAttribute(n, n), n
         }
-    }, k.each(k.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = gt[t] || k.find.attr;
-        gt[t] = function(e, t, n) {
+    }, ce.each(ce.expr.match.bool.source.match(/\w+/g), function(e, t) {
+        var a = xt[t] || ce.find.attr;
+        xt[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = gt[o], gt[o] = r, r = null != a(e, t, n) ? o : null, gt[o] = i), r
+            return n || (i = xt[o], xt[o] = r, r = null != a(e, t, n) ? o : null, xt[o] = i), r
         }
     });
-    var vt = /^(?:input|select|textarea|button)$/i,
-        yt = /^(?:a|area)$/i;
+    var bt = /^(?:input|select|textarea|button)$/i,
+        wt = /^(?:a|area)$/i;
 
-    function mt(e) {
-        return (e.match(R) || []).join(" ")
+    function Tt(e) {
+        return (e.match(D) || []).join(" ")
     }
 
-    function xt(e) {
+    function Ct(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function bt(e) {
-        return Array.isArray(e) ? e : "string" == typeof e && e.match(R) || []
+    function kt(e) {
+        return Array.isArray(e) ? e : "string" == typeof e && e.match(D) || []
     }
-    k.fn.extend({
+    ce.fn.extend({
         prop: function(e, t) {
-            return _(this, k.prop, e, t, 1 < arguments.length)
+            return R(this, ce.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
             return this.each(function() {
-                delete this[k.propFix[e] || e]
+                delete this[ce.propFix[e] || e]
             })
         }
-    }), k.extend({
+    }), ce.extend({
         prop: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && k.isXMLDoc(e) || (t = k.propFix[t] || t, i = k.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
+            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && ce.isXMLDoc(e) || (t = ce.propFix[t] || t, i = ce.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
-                    var t = k.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : vt.test(e.nodeName) || yt.test(e.nodeName) && e.href ? 0 : -1
+                    var t = ce.find.attr(e, "tabindex");
+                    return t ? parseInt(t, 10) : bt.test(e.nodeName) || wt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
-    }), y.optSelected || (k.propHooks.selected = {
+    }), le.optSelected || (ce.propHooks.selected = {
         get: function(e) {
             var t = e.parentNode;
             return t && t.parentNode && t.parentNode.selectedIndex, null
         },
         set: function(e) {
             var t = e.parentNode;
             t && (t.selectedIndex, t.parentNode && t.parentNode.selectedIndex)
         }
-    }), k.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
-        k.propFix[this.toLowerCase()] = this
-    }), k.fn.extend({
+    }), ce.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        ce.propFix[this.toLowerCase()] = this
+    }), ce.fn.extend({
         addClass: function(t) {
-            var e, n, r, i, o, a, s, u = 0;
-            if (m(t)) return this.each(function(e) {
-                k(this).addClass(t.call(this, e, xt(this)))
-            });
-            if ((e = bt(t)).length)
-                while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
-                        a = 0;
-                        while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
-                    } return this
+            var e, n, r, i, o, a;
+            return v(t) ? this.each(function(e) {
+                ce(this).addClass(t.call(this, e, Ct(this)))
+            }) : (e = kt(t)).length ? this.each(function() {
+                if (r = Ct(this), n = 1 === this.nodeType && " " + Tt(r) + " ") {
+                    for (o = 0; o < e.length; o++) i = e[o], n.indexOf(" " + i + " ") < 0 && (n += i + " ");
+                    a = Tt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this
         },
         removeClass: function(t) {
-            var e, n, r, i, o, a, s, u = 0;
-            if (m(t)) return this.each(function(e) {
-                k(this).removeClass(t.call(this, e, xt(this)))
-            });
-            if (!arguments.length) return this.attr("class", "");
-            if ((e = bt(t)).length)
-                while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
-                        a = 0;
-                        while (o = e[a++])
-                            while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
-                    } return this
-        },
-        toggleClass: function(i, t) {
-            var o = typeof i,
-                a = "string" === o || Array.isArray(i);
-            return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                k(this).toggleClass(i.call(this, e, xt(this), t), t)
-            }) : this.each(function() {
-                var e, t, n, r;
-                if (a) {
-                    t = 0, n = k(this), r = bt(i);
-                    while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = xt(this)) && Q.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Q.get(this, "__className__") || ""))
-            })
+            var e, n, r, i, o, a;
+            return v(t) ? this.each(function(e) {
+                ce(this).removeClass(t.call(this, e, Ct(this)))
+            }) : arguments.length ? (e = kt(t)).length ? this.each(function() {
+                if (r = Ct(this), n = 1 === this.nodeType && " " + Tt(r) + " ") {
+                    for (o = 0; o < e.length; o++) {
+                        i = e[o];
+                        while (-1 < n.indexOf(" " + i + " ")) n = n.replace(" " + i + " ", " ")
+                    }
+                    a = Tt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this : this.attr("class", "")
+        },
+        toggleClass: function(t, n) {
+            var e, r, i, o, a = typeof t,
+                s = "string" === a || Array.isArray(t);
+            return v(t) ? this.each(function(e) {
+                ce(this).toggleClass(t.call(this, e, Ct(this), n), n)
+            }) : "boolean" == typeof n && s ? n ? this.addClass(t) : this.removeClass(t) : (e = kt(t), this.each(function() {
+                if (s)
+                    for (o = ce(this), i = 0; i < e.length; i++) r = e[i], o.hasClass(r) ? o.removeClass(r) : o.addClass(r);
+                else void 0 !== t && "boolean" !== a || ((r = Ct(this)) && _.set(this, "__className__", r), this.setAttribute && this.setAttribute("class", r || !1 === t ? "" : _.get(this, "__className__") || ""))
+            }))
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + mt(xt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + Tt(Ct(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var wt = /\r/g;
-    k.fn.extend({
+    var St = /\r/g;
+    ce.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
-            return arguments.length ? (i = m(n), this.each(function(e) {
+            return arguments.length ? (i = v(n), this.each(function(e) {
                 var t;
-                1 === this.nodeType && (null == (t = i ? n.call(this, e, k(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = k.map(t, function(e) {
+                1 === this.nodeType && (null == (t = i ? n.call(this, e, ce(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = ce.map(t, function(e) {
                     return null == e ? "" : e + ""
-                })), (r = k.valHooks[this.type] || k.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = k.valHooks[t.type] || k.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(wt, "") : null == e ? "" : e : void 0
+                })), (r = ce.valHooks[this.type] || ce.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
+            })) : t ? (r = ce.valHooks[t.type] || ce.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(St, "") : null == e ? "" : e : void 0
         }
-    }), k.extend({
+    }), ce.extend({
         valHooks: {
             option: {
                 get: function(e) {
-                    var t = k.find.attr(e, "value");
-                    return null != t ? t : mt(k.text(e))
+                    var t = ce.find.attr(e, "value");
+                    return null != t ? t : Tt(ce.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
                         s = a ? null : [],
                         u = a ? o + 1 : i.length;
                     for (r = o < 0 ? u : a ? o : 0; r < u; r++)
-                        if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !A(n.parentNode, "optgroup"))) {
-                            if (t = k(n).val(), a) return t;
+                        if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !fe(n.parentNode, "optgroup"))) {
+                            if (t = ce(n).val(), a) return t;
                             s.push(t)
                         } return s
                 },
                 set: function(e, t) {
                     var n, r, i = e.options,
-                        o = k.makeArray(t),
+                        o = ce.makeArray(t),
                         a = i.length;
-                    while (a--)((r = i[a]).selected = -1 < k.inArray(k.valHooks.option.get(r), o)) && (n = !0);
+                    while (a--)((r = i[a]).selected = -1 < ce.inArray(ce.valHooks.option.get(r), o)) && (n = !0);
                     return n || (e.selectedIndex = -1), o
                 }
             }
         }
-    }), k.each(["radio", "checkbox"], function() {
-        k.valHooks[this] = {
+    }), ce.each(["radio", "checkbox"], function() {
+        ce.valHooks[this] = {
             set: function(e, t) {
-                if (Array.isArray(t)) return e.checked = -1 < k.inArray(k(e).val(), t)
+                if (Array.isArray(t)) return e.checked = -1 < ce.inArray(ce(e).val(), t)
             }
-        }, y.checkOn || (k.valHooks[this].get = function(e) {
+        }, le.checkOn || (ce.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
-    }), y.focusin = "onfocusin" in C;
-    var Tt = /^(?:focusinfocus|focusoutblur)$/,
-        Ct = function(e) {
+    });
+    var Et = ie.location,
+        jt = {
+            guid: Date.now()
+        },
+        At = /\?/;
+    ce.parseXML = function(e) {
+        var t, n;
+        if (!e || "string" != typeof e) return null;
+        try {
+            t = (new ie.DOMParser).parseFromString(e, "text/xml")
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || ce.error("Invalid XML: " + (n ? ce.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
+    };
+    var Dt = /^(?:focusinfocus|focusoutblur)$/,
+        Nt = function(e) {
             e.stopPropagation()
         };
-    k.extend(k.event, {
+    ce.extend(ce.event, {
         trigger: function(e, t, n, r) {
-            var i, o, a, s, u, l, c, f, p = [n || E],
-                d = v.call(e, "type") ? e.type : e,
-                h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !Tt.test(d + k.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[k.expando] ? e : new k.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : k.makeArray(t, [e]), c = k.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
-                if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, Tt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
-                    a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
+            var i, o, a, s, u, l, c, f, p = [n || C],
+                d = ue.call(e, "type") ? e.type : e,
+                h = ue.call(e, "namespace") ? e.namespace.split(".") : [];
+            if (o = f = a = n = n || C, 3 !== n.nodeType && 8 !== n.nodeType && !Dt.test(d + ce.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[ce.expando] ? e : new ce.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : ce.makeArray(t, [e]), c = ce.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+                if (!r && !c.noBubble && !y(n)) {
+                    for (s = c.delegateType || d, Dt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    a === (n.ownerDocument || C) && p.push(a.defaultView || a.parentWindow || ie)
                 }
                 i = 0;
-                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Q.get(o, "events") || {})[e.type] && Q.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && G(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !G(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), k.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, Ct), n[d](), e.isPropagationStopped() && f.removeEventListener(d, Ct), k.event.triggered = void 0, a && (n[u] = a)), e.result
+                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (_.get(o, "events") || Object.create(null))[e.type] && _.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && $(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !$(n) || u && v(n[d]) && !y(n) && ((a = n[u]) && (n[u] = null), ce.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, Nt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, Nt), ce.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
-            var r = k.extend(new k.Event, n, {
+            var r = ce.extend(new ce.Event, n, {
                 type: e,
                 isSimulated: !0
             });
-            k.event.trigger(r, null, t)
+            ce.event.trigger(r, null, t)
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         trigger: function(e, t) {
             return this.each(function() {
-                k.event.trigger(e, t, this)
+                ce.event.trigger(e, t, this)
             })
         },
         triggerHandler: function(e, t) {
             var n = this[0];
-            if (n) return k.event.trigger(e, t, n, !0)
-        }
-    }), y.focusin || k.each({
-        focus: "focusin",
-        blur: "focusout"
-    }, function(n, r) {
-        var i = function(e) {
-            k.event.simulate(r, e.target, k.event.fix(e))
-        };
-        k.event.special[r] = {
-            setup: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r);
-                t || e.addEventListener(n, i, !0), Q.access(e, r, (t || 0) + 1)
-            },
-            teardown: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r) - 1;
-                t ? Q.access(e, r, t) : (e.removeEventListener(n, i, !0), Q.remove(e, r))
-            }
+            if (n) return ce.event.trigger(e, t, n, !0)
         }
     });
-    var Et = C.location,
-        kt = Date.now(),
-        St = /\?/;
-    k.parseXML = function(e) {
-        var t;
-        if (!e || "string" != typeof e) return null;
-        try {
-            t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {
-            t = void 0
-        }
-        return t && !t.getElementsByTagName("parsererror").length || k.error("Invalid XML: " + e), t
-    };
-    var Nt = /\[\]$/,
-        At = /\r?\n/g,
-        Dt = /^(?:submit|button|image|reset|file)$/i,
-        jt = /^(?:input|select|textarea|keygen)/i;
+    var qt = /\[\]$/,
+        Lt = /\r?\n/g,
+        Ht = /^(?:submit|button|image|reset|file)$/i,
+        Ot = /^(?:input|select|textarea|keygen)/i;
 
-    function qt(n, e, r, i) {
+    function Pt(n, e, r, i) {
         var t;
-        if (Array.isArray(e)) k.each(e, function(e, t) {
-            r || Nt.test(n) ? i(n, t) : qt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+        if (Array.isArray(e)) ce.each(e, function(e, t) {
+            r || qt.test(n) ? i(n, t) : Pt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
-        else if (r || "object" !== w(e)) i(n, e);
+        else if (r || "object" !== x(e)) i(n, e);
         else
-            for (t in e) qt(n + "[" + t + "]", e[t], r, i)
+            for (t in e) Pt(n + "[" + t + "]", e[t], r, i)
     }
-    k.param = function(e, t) {
+    ce.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
-                var n = m(t) ? t() : t;
+                var n = v(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
-        if (Array.isArray(e) || e.jquery && !k.isPlainObject(e)) k.each(e, function() {
+        if (Array.isArray(e) || e.jquery && !ce.isPlainObject(e)) ce.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) qt(n, e[n], t, i);
+            for (n in e) Pt(n, e[n], t, i);
         return r.join("&")
-    }, k.fn.extend({
+    }, ce.fn.extend({
         serialize: function() {
-            return k.param(this.serializeArray())
+            return ce.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
-                var e = k.prop(this, "elements");
-                return e ? k.makeArray(e) : this
+                var e = ce.prop(this, "elements");
+                return e ? ce.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !k(this).is(":disabled") && jt.test(this.nodeName) && !Dt.test(e) && (this.checked || !pe.test(e))
+                return this.name && !ce(this).is(":disabled") && Ot.test(this.nodeName) && !Ht.test(e) && (this.checked || !we.test(e))
             }).map(function(e, t) {
-                var n = k(this).val();
-                return null == n ? null : Array.isArray(n) ? k.map(n, function(e) {
+                var n = ce(this).val();
+                return null == n ? null : Array.isArray(n) ? ce.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(At, "\r\n")
+                        value: e.replace(Lt, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(At, "\r\n")
+                    value: n.replace(Lt, "\r\n")
                 }
             }).get()
         }
     });
-    var Lt = /%20/g,
-        Ht = /#.*$/,
-        Ot = /([?&])_=[^&]*/,
-        Pt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Rt = /^(?:GET|HEAD)$/,
-        Mt = /^\/\//,
-        It = {},
-        Wt = {},
-        $t = "*/".concat("*"),
-        Ft = E.createElement("a");
+    var Rt = /%20/g,
+        Mt = /#.*$/,
+        It = /([?&])_=[^&]*/,
+        Wt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Ft = /^(?:GET|HEAD)$/,
+        $t = /^\/\//,
+        Bt = {},
+        _t = {},
+        Xt = "*/".concat("*"),
+        Ut = C.createElement("a");
 
-    function Bt(o) {
+    function zt(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
-                i = e.toLowerCase().match(R) || [];
-            if (m(t))
+                i = e.toLowerCase().match(D) || [];
+            if (v(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function _t(t, i, o, a) {
+    function Vt(t, i, o, a) {
         var s = {},
-            u = t === Wt;
+            u = t === _t;
 
         function l(e) {
             var r;
-            return s[e] = !0, k.each(t[e] || [], function(e, t) {
+            return s[e] = !0, ce.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function zt(e, t) {
-        var n, r, i = k.ajaxSettings.flatOptions || {};
+    function Gt(e, t) {
+        var n, r, i = ce.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
-        return r && k.extend(!0, e, r), e
+        return r && ce.extend(!0, e, r), e
     }
-    Ft.href = Et.href, k.extend({
+    Ut.href = Et.href, ce.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
             url: Et.href,
             type: "GET",
             isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Et.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": $t,
+                "*": Xt,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2773,45 +2733,45 @@
                 text: "responseText",
                 json: "responseJSON"
             },
             converters: {
                 "* text": String,
                 "text html": !0,
                 "text json": JSON.parse,
-                "text xml": k.parseXML
+                "text xml": ce.parseXML
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? zt(zt(e, k.ajaxSettings), t) : zt(k.ajaxSettings, e)
+            return t ? Gt(Gt(e, ce.ajaxSettings), t) : Gt(ce.ajaxSettings, e)
         },
-        ajaxPrefilter: Bt(It),
-        ajaxTransport: Bt(Wt),
+        ajaxPrefilter: zt(Bt),
+        ajaxTransport: zt(_t),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
-            var c, f, p, n, d, r, h, g, i, o, v = k.ajaxSetup({}, t),
+            var c, f, p, n, d, r, h, g, i, o, v = ce.ajaxSetup({}, t),
                 y = v.context || v,
-                m = v.context && (y.nodeType || y.jquery) ? k(y) : k.event,
-                x = k.Deferred(),
-                b = k.Callbacks("once memory"),
+                m = v.context && (y.nodeType || y.jquery) ? ce(y) : ce.event,
+                x = ce.Deferred(),
+                b = ce.Callbacks("once memory"),
                 w = v.statusCode || {},
                 a = {},
                 s = {},
                 u = "canceled",
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = Pt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = Wt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2831,41 +2791,41 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || Et.href) + "").replace(Mt, Et.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(R) || [""], null == v.crossDomain) {
-                r = E.createElement("a");
+            if (x.promise(T), v.url = ((e || v.url || Et.href) + "").replace($t, Et.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(D) || [""], null == v.crossDomain) {
+                r = C.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Ft.protocol + "//" + Ft.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Ut.protocol + "//" + Ut.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = k.param(v.data, v.traditional)), _t(It, v, t, T), h) return T;
-            for (i in (g = k.event && v.global) && 0 == k.active++ && k.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Rt.test(v.type), f = v.url.replace(Ht, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Lt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (St.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Ot, "$1"), o = (St.test(f) ? "&" : "?") + "_=" + kt++ + o), v.url = f + o), v.ifModified && (k.lastModified[f] && T.setRequestHeader("If-Modified-Since", k.lastModified[f]), k.etag[f] && T.setRequestHeader("If-None-Match", k.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + $t + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = ce.param(v.data, v.traditional)), Vt(Bt, v, t, T), h) return T;
+            for (i in (g = ce.event && v.global) && 0 == ce.active++ && ce.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ft.test(v.type), f = v.url.replace(Mt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Rt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (At.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(It, "$1"), o = (At.test(f) ? "&" : "?") + "_=" + jt.guid++ + o), v.url = f + o), v.ifModified && (ce.lastModified[f] && T.setRequestHeader("If-Modified-Since", ce.lastModified[f]), ce.etag[f] && T.setRequestHeader("If-None-Match", ce.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + Xt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = _t(Wt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Vt(_t, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
-                v.async && 0 < v.timeout && (d = C.setTimeout(function() {
+                v.async && 0 < v.timeout && (d = ie.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
                     if (h) throw e;
                     l(-1, e)
                 }
             } else l(-1, "No Transport");
 
             function l(e, t, n, r) {
                 var i, o, a, s, u, l = t;
-                h || (h = !0, d && C.clearTimeout(d), c = void 0, p = r || "", T.readyState = 0 < e ? 4 : 0, i = 200 <= e && e < 300 || 304 === e, n && (s = function(e, t, n) {
+                h || (h = !0, d && ie.clearTimeout(d), c = void 0, p = r || "", T.readyState = 0 < e ? 4 : 0, i = 200 <= e && e < 300 || 304 === e, n && (s = function(e, t, n) {
                     var r, i, o, a, s = e.contents,
                         u = e.dataTypes;
                     while ("*" === u[0]) u.shift(), void 0 === r && (r = e.mimeType || t.getResponseHeader("Content-Type"));
                     if (r)
                         for (i in s)
                             if (s[i] && s[i].test(r)) {
                                 u.unshift(i);
@@ -2878,15 +2838,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < ce.inArray("script", v.dataTypes) && ce.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -2908,209 +2868,208 @@
                                 }
                             }
                     }
                     return {
                         state: "success",
                         data: t
                     }
-                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (k.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (k.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --k.active || k.event.trigger("ajaxStop")))
+                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (ce.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (ce.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --ce.active || ce.event.trigger("ajaxStop")))
             }
             return T
         },
         getJSON: function(e, t, n) {
-            return k.get(e, t, n, "json")
+            return ce.get(e, t, n, "json")
         },
         getScript: function(e, t) {
-            return k.get(e, void 0, t, "script")
+            return ce.get(e, void 0, t, "script")
         }
-    }), k.each(["get", "post"], function(e, i) {
-        k[i] = function(e, t, n, r) {
-            return m(t) && (r = r || n, n = t, t = void 0), k.ajax(k.extend({
+    }), ce.each(["get", "post"], function(e, i) {
+        ce[i] = function(e, t, n, r) {
+            return v(t) && (r = r || n, n = t, t = void 0), ce.ajax(ce.extend({
                 url: e,
                 type: i,
                 dataType: r,
                 data: t,
                 success: n
-            }, k.isPlainObject(e) && e))
+            }, ce.isPlainObject(e) && e))
         }
-    }), k._evalUrl = function(e, t) {
-        return k.ajax({
+    }), ce.ajaxPrefilter(function(e) {
+        var t;
+        for (t in e.headers) "content-type" === t.toLowerCase() && (e.contentType = e.headers[t] || "")
+    }), ce._evalUrl = function(e, t, n) {
+        return ce.ajax({
             url: e,
             type: "GET",
             dataType: "script",
             cache: !0,
             async: !1,
             global: !1,
             converters: {
                 "text script": function() {}
             },
             dataFilter: function(e) {
-                k.globalEval(e, t)
+                ce.globalEval(e, t, n)
             }
         })
-    }, k.fn.extend({
+    }, ce.fn.extend({
         wrapAll: function(e) {
             var t;
-            return this[0] && (m(e) && (e = e.call(this[0])), t = k(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
+            return this[0] && (v(e) && (e = e.call(this[0])), t = ce(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
                 var e = this;
                 while (e.firstElementChild) e = e.firstElementChild;
                 return e
             }).append(this)), this
         },
         wrapInner: function(n) {
-            return m(n) ? this.each(function(e) {
-                k(this).wrapInner(n.call(this, e))
+            return v(n) ? this.each(function(e) {
+                ce(this).wrapInner(n.call(this, e))
             }) : this.each(function() {
-                var e = k(this),
+                var e = ce(this),
                     t = e.contents();
                 t.length ? t.wrapAll(n) : e.append(n)
             })
         },
         wrap: function(t) {
-            var n = m(t);
+            var n = v(t);
             return this.each(function(e) {
-                k(this).wrapAll(n ? t.call(this, e) : t)
+                ce(this).wrapAll(n ? t.call(this, e) : t)
             })
         },
         unwrap: function(e) {
             return this.parent(e).not("body").each(function() {
-                k(this).replaceWith(this.childNodes)
+                ce(this).replaceWith(this.childNodes)
             }), this
         }
-    }), k.expr.pseudos.hidden = function(e) {
-        return !k.expr.pseudos.visible(e)
-    }, k.expr.pseudos.visible = function(e) {
+    }), ce.expr.pseudos.hidden = function(e) {
+        return !ce.expr.pseudos.visible(e)
+    }, ce.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
-    }, k.ajaxSettings.xhr = function() {
+    }, ce.ajaxSettings.xhr = function() {
         try {
-            return new C.XMLHttpRequest
+            return new ie.XMLHttpRequest
         } catch (e) {}
     };
-    var Ut = {
+    var Yt = {
             0: 200,
             1223: 204
         },
-        Xt = k.ajaxSettings.xhr();
-    y.cors = !!Xt && "withCredentials" in Xt, y.ajax = Xt = !!Xt, k.ajaxTransport(function(i) {
+        Qt = ce.ajaxSettings.xhr();
+    le.cors = !!Qt && "withCredentials" in Qt, le.ajax = Qt = !!Qt, ce.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || Xt && !i.crossDomain) return {
+        if (le.cors || Qt && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Ut[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Yt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
-                    4 === r.readyState && C.setTimeout(function() {
+                    4 === r.readyState && ie.setTimeout(function() {
                         o && a()
                     })
                 }, o = o("abort");
                 try {
                     r.send(i.hasContent && i.data || null)
                 } catch (e) {
                     if (o) throw e
                 }
             },
             abort: function() {
                 o && o()
             }
         }
-    }), k.ajaxPrefilter(function(e) {
+    }), ce.ajaxPrefilter(function(e) {
         e.crossDomain && (e.contents.script = !1)
-    }), k.ajaxSetup({
+    }), ce.ajaxSetup({
         accepts: {
             script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
         },
         contents: {
             script: /\b(?:java|ecma)script\b/
         },
         converters: {
             "text script": function(e) {
-                return k.globalEval(e), e
+                return ce.globalEval(e), e
             }
         }
-    }), k.ajaxPrefilter("script", function(e) {
+    }), ce.ajaxPrefilter("script", function(e) {
         void 0 === e.cache && (e.cache = !1), e.crossDomain && (e.type = "GET")
-    }), k.ajaxTransport("script", function(n) {
+    }), ce.ajaxTransport("script", function(n) {
         var r, i;
         if (n.crossDomain || n.scriptAttrs) return {
             send: function(e, t) {
-                r = k("<script>").attr(n.scriptAttrs || {}).prop({
+                r = ce("<script>").attr(n.scriptAttrs || {}).prop({
                     charset: n.scriptCharset,
                     src: n.url
                 }).on("load error", i = function(e) {
                     r.remove(), i = null, e && t("error" === e.type ? 404 : 200, e.type)
-                }), E.head.appendChild(r[0])
+                }), C.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var Vt, Gt = [],
-        Yt = /(=)\?(?=&|$)|\?\?/;
-    k.ajaxSetup({
+    var Jt, Kt = [],
+        Zt = /(=)\?(?=&|$)|\?\?/;
+    ce.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = Gt.pop() || k.expando + "_" + kt++;
+            var e = Kt.pop() || ce.expando + "_" + jt.guid++;
             return this[e] = !0, e
         }
-    }), k.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Yt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Yt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Yt, "$1" + r) : !1 !== e.jsonp && (e.url += (St.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
-            return o || k.error(r + " was not called"), o[0]
-        }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
+    }), ce.ajaxPrefilter("json jsonp", function(e, t, n) {
+        var r, i, o, a = !1 !== e.jsonp && (Zt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Zt.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = v(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Zt, "$1" + r) : !1 !== e.jsonp && (e.url += (At.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+            return o || ce.error(r + " was not called"), o[0]
+        }, e.dataTypes[0] = "json", i = ie[r], ie[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? k(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Gt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? ce(ie).removeProp(r) : ie[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Kt.push(r)), o && v(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((Vt = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Vt.childNodes.length), k.parseHTML = function(e, t, n) {
-        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = D.exec(e)) ? [t.createElement(i[1])] : (i = we([e], t, o), o && o.length && k(o).remove(), k.merge([], i.childNodes)));
+    }), le.createHTMLDocument = ((Jt = C.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Jt.childNodes.length), ce.parseHTML = function(e, t, n) {
+        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (le.createHTMLDocument ? ((r = (t = C.implementation.createHTMLDocument("")).createElement("base")).href = C.location.href, t.head.appendChild(r)) : t = C), o = !n && [], (i = w.exec(e)) ? [t.createElement(i[1])] : (i = Ae([e], t, o), o && o.length && ce(o).remove(), ce.merge([], i.childNodes)));
         var r, i, o
-    }, k.fn.load = function(e, t, n) {
+    }, ce.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = mt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && k.ajax({
+        return -1 < s && (r = Tt(e.slice(s)), e = e.slice(0, s)), v(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && ce.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
-            o = arguments, a.html(r ? k("<div>").append(k.parseHTML(e)).find(r) : e)
+            o = arguments, a.html(r ? ce("<div>").append(ce.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
             a.each(function() {
                 n.apply(this, o || [e.responseText, t, e])
             })
         }), this
-    }, k.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
-        k.fn[t] = function(e) {
-            return this.on(t, e)
-        }
-    }), k.expr.pseudos.animated = function(t) {
-        return k.grep(k.timers, function(e) {
+    }, ce.expr.pseudos.animated = function(t) {
+        return ce.grep(ce.timers, function(e) {
             return t === e.elem
         }).length
-    }, k.offset = {
+    }, ce.offset = {
         setOffset: function(e, t, n) {
-            var r, i, o, a, s, u, l = k.css(e, "position"),
-                c = k(e),
+            var r, i, o, a, s, u, l = ce.css(e, "position"),
+                c = ce(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = k.css(e, "top"), u = k.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, k.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = ce.css(e, "top"), u = ce.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), v(t) && (t = t.call(e, n, ce.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
         }
-    }, k.fn.extend({
+    }, ce.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
-                k.offset.setOffset(this, t, e)
+                ce.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
             return r ? r.getClientRects().length ? (e = r.getBoundingClientRect(), n = r.ownerDocument.defaultView, {
                 top: e.top + n.pageYOffset,
                 left: e.left + n.pageXOffset
             }) : {
                 top: 0,
@@ -3120,100 +3079,107 @@
         position: function() {
             if (this[0]) {
                 var e, t, n, r = this[0],
                     i = {
                         top: 0,
                         left: 0
                     };
-                if ("fixed" === k.css(r, "position")) t = r.getBoundingClientRect();
+                if ("fixed" === ce.css(r, "position")) t = r.getBoundingClientRect();
                 else {
                     t = this.offset(), n = r.ownerDocument, e = r.offsetParent || n.documentElement;
-                    while (e && (e === n.body || e === n.documentElement) && "static" === k.css(e, "position")) e = e.parentNode;
-                    e && e !== r && 1 === e.nodeType && ((i = k(e).offset()).top += k.css(e, "borderTopWidth", !0), i.left += k.css(e, "borderLeftWidth", !0))
+                    while (e && (e === n.body || e === n.documentElement) && "static" === ce.css(e, "position")) e = e.parentNode;
+                    e && e !== r && 1 === e.nodeType && ((i = ce(e).offset()).top += ce.css(e, "borderTopWidth", !0), i.left += ce.css(e, "borderLeftWidth", !0))
                 }
                 return {
-                    top: t.top - i.top - k.css(r, "marginTop", !0),
-                    left: t.left - i.left - k.css(r, "marginLeft", !0)
+                    top: t.top - i.top - ce.css(r, "marginTop", !0),
+                    left: t.left - i.left - ce.css(r, "marginLeft", !0)
                 }
             }
         },
         offsetParent: function() {
             return this.map(function() {
                 var e = this.offsetParent;
-                while (e && "static" === k.css(e, "position")) e = e.offsetParent;
-                return e || ie
+                while (e && "static" === ce.css(e, "position")) e = e.offsetParent;
+                return e || J
             })
         }
-    }), k.each({
+    }), ce.each({
         scrollLeft: "pageXOffset",
         scrollTop: "pageYOffset"
     }, function(t, i) {
         var o = "pageYOffset" === i;
-        k.fn[t] = function(e) {
-            return _(this, function(e, t, n) {
+        ce.fn[t] = function(e) {
+            return R(this, function(e, t, n) {
                 var r;
-                if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
+                if (y(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
-    }), k.each(["top", "left"], function(e, n) {
-        k.cssHooks[n] = ze(y.pixelPosition, function(e, t) {
-            if (t) return t = _e(e, n), $e.test(t) ? k(e).position()[n] + "px" : t
+    }), ce.each(["top", "left"], function(e, n) {
+        ce.cssHooks[n] = Ye(le.pixelPosition, function(e, t) {
+            if (t) return t = Ge(e, n), _e.test(t) ? ce(e).position()[n] + "px" : t
         })
-    }), k.each({
+    }), ce.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
-        k.each({
+        ce.each({
             padding: "inner" + a,
             content: s,
             "": "outer" + a
         }, function(r, o) {
-            k.fn[o] = function(e, t) {
+            ce.fn[o] = function(e, t) {
                 var n = arguments.length && (r || "boolean" != typeof e),
                     i = r || (!0 === e || !0 === t ? "margin" : "border");
-                return _(this, function(e, t, n) {
+                return R(this, function(e, t, n) {
                     var r;
-                    return x(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? k.css(e, t, i) : k.style(e, t, n, i)
+                    return y(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? ce.css(e, t, i) : ce.style(e, t, n, i)
                 }, s, n ? e : void 0, n)
             }
         })
-    }), k.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
-        k.fn[n] = function(e, t) {
-            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
-        }
-    }), k.fn.extend({
-        hover: function(e, t) {
-            return this.mouseenter(e).mouseleave(t || e)
+    }), ce.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
+        ce.fn[t] = function(e) {
+            return this.on(t, e)
         }
-    }), k.fn.extend({
+    }), ce.fn.extend({
         bind: function(e, t, n) {
             return this.on(e, null, t, n)
         },
         unbind: function(e, t) {
             return this.off(e, null, t)
         },
         delegate: function(e, t, n, r) {
             return this.on(t, e, n, r)
         },
         undelegate: function(e, t, n) {
             return 1 === arguments.length ? this.off(e, "**") : this.off(t, e || "**", n)
+        },
+        hover: function(e, t) {
+            return this.mouseenter(e).mouseleave(t || e)
+        }
+    }), ce.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
+        ce.fn[n] = function(e, t) {
+            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
         }
-    }), k.proxy = function(e, t) {
+    });
+    var en = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+    ce.proxy = function(e, t) {
         var n, r, i;
-        if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
-            return e.apply(t || this, r.concat(s.call(arguments)))
-        }).guid = e.guid = e.guid || k.guid++, i
-    }, k.holdReady = function(e) {
-        e ? k.readyWait++ : k.ready(!0)
-    }, k.isArray = Array.isArray, k.parseJSON = JSON.parse, k.nodeName = A, k.isFunction = m, k.isWindow = x, k.camelCase = V, k.type = w, k.now = Date.now, k.isNumeric = function(e) {
-        var t = k.type(e);
+        if ("string" == typeof t && (n = e[t], t = e, e = n), v(e)) return r = ae.call(arguments, 2), (i = function() {
+            return e.apply(t || this, r.concat(ae.call(arguments)))
+        }).guid = e.guid = e.guid || ce.guid++, i
+    }, ce.holdReady = function(e) {
+        e ? ce.readyWait++ : ce.ready(!0)
+    }, ce.isArray = Array.isArray, ce.parseJSON = JSON.parse, ce.nodeName = fe, ce.isFunction = v, ce.isWindow = y, ce.camelCase = F, ce.type = x, ce.now = Date.now, ce.isNumeric = function(e) {
+        var t = ce.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
+    }, ce.trim = function(e) {
+        return null == e ? "" : (e + "").replace(en, "$1")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
-        return k
+        return ce
     });
-    var Qt = C.jQuery,
-        Jt = C.$;
-    return k.noConflict = function(e) {
-        return C.$ === k && (C.$ = Jt), e && C.jQuery === k && (C.jQuery = Qt), k
-    }, e || (C.jQuery = C.$ = k), k
+    var tn = ie.jQuery,
+        nn = ie.$;
+    return ce.noConflict = function(e) {
+        return ie.$ === ce && (ie.$ = nn), e && ie.jQuery === ce && (ie.jQuery = tn), ce
+    }, "undefined" == typeof e && (ie.jQuery = ie.$ = ce), ce
 });
```

### Comparing `monopyly-1.3.0/monopyly/static/css/style.css` & `monopyly-1.3.1/monopyly/static/css/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 /*-------------------------------------------*/
 
 
 /* Define custom colors for consistent branding */
 :root {
   --moneytree: #5e8f40;
   --moneytree-leaves: #85bb65;
+  --masthead-height: 50px;
 }
 
 html {
   height: 100%;
 }
 
 body {
@@ -80,15 +81,15 @@
  */
 header#masthead {
   position: fixed;
   top: 0;
   z-index: 99;
   display: flex;
   align-items: center;
-  height: 50px;
+  height: var(--masthead-height);
   width: 100%;
   border-width: 0 0 4px 3px;
   border-style: solid;
   border-color: var(--moneytree-leaves);
   background-color: #2b2b2b;
   opacity: 0.9;
 }
@@ -168,15 +169,15 @@
 
 /*
  * Handle the main body content area for pages
  */
 #page {
   display: flex;
   justify-content: space-between;
-  margin-top: 50px;
+  margin-top: var(--masthead-height);
   padding-top: 50px;
   padding-bottom: 30px;
 }
 
 #page .container {
   width: 80%;
 }
@@ -385,14 +386,15 @@
 
 form button:hover,
 form input.button:hover {
   filter: brightness(0.98);
 }
 
 form button:disabled,
+form input:disabled,
 form input.button:disabled {
   color: #bbbbbb;
   filter: brightness(0.95);
 }
 
 form button .icon {
   height: 40px;
```

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-114.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-114.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-120.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-120.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-144.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-144.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-150.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-150.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-152.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-152.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-16.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-16.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-160.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-160.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-180.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-180.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-192.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-192.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-310.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-310.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-32.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-32.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-57.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-57.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-60.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-60.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-64.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-64.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-70.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-70.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-72.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-72.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-76.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-76.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon-96.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon-96.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon.ico` & `monopyly-1.3.1/monopyly/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/favicon/favicon.png` & `monopyly-1.3.1/monopyly/static/favicon/favicon.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/statement.png` & `monopyly-1.3.1/monopyly/static/img/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/bank-account-details.png` & `monopyly-1.3.1/monopyly/static/img/about/bank-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/bank-account-summaries.png` & `monopyly-1.3.1/monopyly/static/img/about/bank-account-summaries.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/bank-accounts.png` & `monopyly-1.3.1/monopyly/static/img/about/bank-accounts.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/credit-account-details.png` & `monopyly-1.3.1/monopyly/static/img/about/credit-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/credit-transactions.png` & `monopyly-1.3.1/monopyly/static/img/about/credit-transactions.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/homepage-user.png` & `monopyly-1.3.1/monopyly/static/img/about/homepage-user.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/homepage.png` & `monopyly-1.3.1/monopyly/static/img/about/homepage.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/about/statement-details.png` & `monopyly-1.3.1/monopyly/static/img/about/statement-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/cards/chase-card.png` & `monopyly-1.3.1/monopyly/static/img/cards/chase-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/cards/discover-card.png` & `monopyly-1.3.1/monopyly/static/img/cards/discover-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/cards/new-card.png` & `monopyly-1.3.1/monopyly/static/img/cards/new-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/cards/template-card.png` & `monopyly-1.3.1/monopyly/static/img/cards/template-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/arrow-down.png` & `monopyly-1.3.1/monopyly/static/img/icons/arrow-down.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/arrow-left.png` & `monopyly-1.3.1/monopyly/static/img/icons/arrow-left.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/arrow-up.png` & `monopyly-1.3.1/monopyly/static/img/icons/arrow-up.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/checkmark.png` & `monopyly-1.3.1/monopyly/static/img/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/delete-orange-thick.png` & `monopyly-1.3.1/monopyly/static/img/icons/delete-orange-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/delete-orange.png` & `monopyly-1.3.1/monopyly/static/img/icons/delete-orange.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/delete-thick.png` & `monopyly-1.3.1/monopyly/static/img/icons/delete-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/delete.png` & `monopyly-1.3.1/monopyly/static/img/icons/delete.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/edit.png` & `monopyly-1.3.1/monopyly/static/img/icons/edit.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/link.png` & `monopyly-1.3.1/monopyly/static/img/icons/link.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/minus-thick.png` & `monopyly-1.3.1/monopyly/static/img/icons/minus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/minus.png` & `monopyly-1.3.1/monopyly/static/img/icons/minus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/plus-thick.png` & `monopyly-1.3.1/monopyly/static/img/icons/plus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/plus.png` & `monopyly-1.3.1/monopyly/static/img/icons/plus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/refresh.png` & `monopyly-1.3.1/monopyly/static/img/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/save.png` & `monopyly-1.3.1/monopyly/static/img/icons/save.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/sort-asc.png` & `monopyly-1.3.1/monopyly/static/img/icons/sort-asc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/sort-desc.png` & `monopyly-1.3.1/monopyly/static/img/icons/sort-desc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/statement.png` & `monopyly-1.3.1/monopyly/static/img/icons/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/img/icons/x-thick.png` & `monopyly-1.3.1/monopyly/static/img/icons/x-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/add_subtransaction.js` & `monopyly-1.3.1/monopyly/static/js/add_subtransaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/add_transfer.js` & `monopyly-1.3.1/monopyly/static/js/add_transfer.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,30 @@
     }
 
     /**
      * Add the subform.
      */
     addSubform(response) {
         $('.add-info.buttons').after(response);
+        // Disable the merchant field (it is replaced by the linked bank name)
+        $('input#merchant').val("");
+        $('input#merchant').prop("disabled", true);
+    }
+
+    /**
+     */
+    disableMerchantField() {}
+
+    /**
+     * Remove the subform
+     */
+    removeSubform($subform) {
+        $subform.remove();
+        // Reenable the merchant field
+        $('input#merchant').prop("disabled", false);
     }
 
 }
 
 (function() {
 
     const subformManager = new BankTransferSubformManager();
```

### Comparing `monopyly-1.3.0/monopyly/static/js/autocomplete_transaction.js` & `monopyly-1.3.1/monopyly/static/js/autocomplete_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/bind_tag_actions.js` & `monopyly-1.3.1/monopyly/static/js/bind_tag_actions.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/define_filter.js` & `monopyly-1.3.1/monopyly/static/js/define_filter.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/display_new_account_type_inputs.js` & `monopyly-1.3.1/monopyly/static/js/display_new_account_type_inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/display_new_credit_account_inputs.js` & `monopyly-1.3.1/monopyly/static/js/display_new_credit_account_inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/expand_bank.js` & `monopyly-1.3.1/monopyly/static/js/expand_bank.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/expand_bank_account.js` & `monopyly-1.3.1/monopyly/static/js/expand_bank_account.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/expand_transaction.js` & `monopyly-1.3.1/monopyly/static/js/expand_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/flip_card.js` & `monopyly-1.3.1/monopyly/static/js/flip_card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/infer_card.js` & `monopyly-1.3.1/monopyly/static/js/infer_card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/infer_statement.js` & `monopyly-1.3.1/monopyly/static/js/infer_statement.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/make_payment.js` & `monopyly-1.3.1/monopyly/static/js/make_payment.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/show_linked_transaction.js` & `monopyly-1.3.1/monopyly/static/js/show_linked_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_account_statement_parameters.js` & `monopyly-1.3.1/monopyly/static/js/update_account_statement_parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_bank_name.js` & `monopyly-1.3.1/monopyly/static/js/update_bank_name.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_card_status.js` & `monopyly-1.3.1/monopyly/static/js/update_card_status.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_statement_parameters.js` & `monopyly-1.3.1/monopyly/static/js/update_statement_parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_statements_display.js` & `monopyly-1.3.1/monopyly/static/js/update_statements_display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/update_transactions_display.js` & `monopyly-1.3.1/monopyly/static/js/update_transactions_display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/autocomplete_input.js` & `monopyly-1.3.1/monopyly/static/js/modules/autocomplete_input.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/expand_box_row.js` & `monopyly-1.3.1/monopyly/static/js/modules/expand_box_row.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/expand_transaction.js` & `monopyly-1.3.1/monopyly/static/js/modules/expand_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/manage_acquisition_form.js` & `monopyly-1.3.1/monopyly/static/js/modules/manage_acquisition_form.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/manage_overlays.js` & `monopyly-1.3.1/monopyly/static/js/modules/manage_overlays.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/manage_subforms.js` & `monopyly-1.3.1/monopyly/static/js/modules/manage_subforms.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -52,26 +52,33 @@
     #executeAjaxRequest() {
         const rawData = this.determineAjaxData();
         const callback = this.#handleAjaxResponse.bind(this);
         executeAjaxRequest(this.addFormEndpoint, rawData, callback);
     }
 
     /**
+     * Remove the subform
+     */
+    removeSubform($subform) {
+        $subform.remove();
+    }
+
+    /**
      * Provide an AJAX callback that adds a subform and binds the remove button.
      */
     #handleAjaxResponse(response) {
         this.addSubform(response);
         if (this.toggleButton) {
             this.$addFormButton.hide();
         }
 
         const $removeButtons = $(".subform .close.button");
         const manager = this;
         $removeButtons.on("click", function() {
-            this.closest(".subform").remove();
+            manager.removeSubform(this.closest(".subform"));
             if (manager.toggleButton) {
                 manager.$addFormButton.show();
             }
         });
     }
 
 }
```

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/update_database_widget.js` & `monopyly-1.3.1/monopyly/static/js/modules/update_database_widget.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/static/js/modules/update_display_ajax.js` & `monopyly-1.3.1/monopyly/static/js/modules/update_display_ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/index.html` & `monopyly-1.3.1/monopyly/templates/index.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/layout.html` & `monopyly-1.3.1/monopyly/templates/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     <link rel="apple-touch-icon" sizes="152x152" href="{{ url_for('static', filename='favicon/favicon-152.png') }}">
     <link rel="apple-touch-icon" sizes="180x180" href="{{ url_for('static', filename='favicon/favicon-180.png') }}">
     <meta name="msapplication-TileColor" content="#FFFFFF">
     <meta name="msapplication-TileImage" content="{{ url_for('static', filename='favicon/favicon-144.png') }}">
     <meta name="msapplication-config" content="{{ url_for('static', filename='favicon/browserconfig.xml') }}">
     <!-- ****** faviconit.com favicons ****** -->
     <!-- Use Google JQuery CDN -->
-    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
-    <script>window.jQuery || document.write('<script src="{{ url_for('static', filename='jquery-3.4.1.js') }}"><\/script>')</script>
+    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.0/jquery.min.js"></script>
+    <script>window.jQuery || document.write('<script src="{{ url_for('static', filename='jquery-3.7.0.min.js') }}"><\/script>')</script>
   </head>
   <body>
 
     <header id="masthead">
       <div class="container">
 
         <a href="{{ url_for('core.index') }}">
@@ -85,15 +85,15 @@
         {% block right_sidebar %}{% endblock %}
       </aside>
 
     </div>
 
     <footer id="site-info">
       <p>
-        <span id="version"><i>Monopyly</i> {{ monopyly_version }}</span>
+        <span id="version"><i>Monopyly</i> {{ app_version }}</span>
         –
         <span id="copyright">{{ copyright_statement }}, Mitch Negus</span>
         </p>
     </footer>
 
     {% block javascript %}{% endblock %}
```

#### html2text {}

```diff
@@ -32,9 +32,9 @@
 {% endif %}
 
  {% block left_sidebar %}{% endblock %}    {% block header %}{% endblock %}  {%
 for message in get_flashed_messages() %}
 {{ message }}
 {% endfor %} {% block content %}{% endblock %}   {% block right_sidebar %}{%
 endblock %}
-Monopyly {{ monopyly_version }} â {{ copyright_statement }}, Mitch Negus
+Monopyly {{ app_version }} â {{ copyright_statement }}, Mitch Negus
  {% block javascript %}{% endblock %}
```

### Comparing `monopyly-1.3.0/monopyly/templates/profile.html` & `monopyly-1.3.1/monopyly/templates/profile.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/story.html` & `monopyly-1.3.1/monopyly/templates/story.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/account_page.html` & `monopyly-1.3.1/monopyly/templates/banking/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/account_summaries.html` & `monopyly-1.3.1/monopyly/templates/banking/account_summaries.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/account_summaries_page.html` & `monopyly-1.3.1/monopyly/templates/banking/account_summaries_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/accounts_page.html` & `monopyly-1.3.1/monopyly/templates/banking/accounts_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/account_form/account_form.html` & `monopyly-1.3.1/monopyly/templates/banking/account_form/account_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/account_form/account_form_page_new.html` & `monopyly-1.3.1/monopyly/templates/banking/account_form/account_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/transaction_form/bank_info_form.html` & `monopyly-1.3.1/monopyly/templates/banking/transaction_form/bank_info_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form.html` & `monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page.html` & `monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/banking/transactions_table/expanded_row_content.html` & `monopyly-1.3.1/monopyly/templates/banking/transactions_table/expanded_row_content.html`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,29 @@
     </div>
   </div>
 
   <div class="description">
 
     <div class="description-header">
       <div class="brief">
-        {% if transaction.merchant %}
-            {% set merchant_reference = ": " + transaction.merchant %}
+        {% if transaction | is_single_bank_transfer %}
+            Transfer
         {% else %}
-            {% set merchant_reference = "" %}
-        {% endif %}
-        {% if transaction.total > 0 %}
-          Deposit{{ merchant_reference }}
-        {% elif transaction.total < 0 %}
-          Withdrawal{{ merchant_reference }}
-        {% else %}
-          Exchange
+          {% if transaction.merchant %}
+              {% set merchant_reference = ": " + transaction.merchant %}
+          {% else %}
+              {% set merchant_reference = "" %}
+          {% endif %}
+          {% if transaction.total > 0 %}
+            Deposit{{ merchant_reference }}
+          {% elif transaction.total < 0 %}
+            Withdrawal{{ merchant_reference }}
+          {% else %}
+            Exchange
+          {% endif %}
         {% endif %}
 
       </div>
       <div class="total">
         ${{ transaction.total|currency }}
       </div>
     </div>
```

### Comparing `monopyly-1.3.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html` & `monopyly-1.3.1/monopyly/templates/banking/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/common/transaction_form/subtransaction_subform.html` & `monopyly-1.3.1/monopyly/templates/common/transaction_form/subtransaction_subform.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html` & `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_bank_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html` & `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_credit_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html` & `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_transaction_overlay.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_expanded.html` & `monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_expanded.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/account_page.html` & `monopyly-1.3.1/monopyly/templates/credit/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/cards.html` & `monopyly-1.3.1/monopyly/templates/credit/cards.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/statement_page.html` & `monopyly-1.3.1/monopyly/templates/credit/statement_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/statement_summary.html` & `monopyly-1.3.1/monopyly/templates/credit/statement_summary.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/statements.html` & `monopyly-1.3.1/monopyly/templates/credit/statements.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/statements_page.html` & `monopyly-1.3.1/monopyly/templates/credit/statements_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/tags_page.html` & `monopyly-1.3.1/monopyly/templates/credit/tags_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transaction_submission_page.html` & `monopyly-1.3.1/monopyly/templates/credit/transaction_submission_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transactions_page.html` & `monopyly-1.3.1/monopyly/templates/credit/transactions_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/card_form/card_form.html` & `monopyly-1.3.1/monopyly/templates/credit/card_form/card_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/card_form/card_form_page_new.html` & `monopyly-1.3.1/monopyly/templates/credit/card_form/card_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html` & `monopyly-1.3.1/monopyly/templates/credit/card_form/transfer_statement_inquiry.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_back.html` & `monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_back.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_front.html` & `monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_front.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/tag_tree/subtag_tree.html` & `monopyly-1.3.1/monopyly/templates/credit/tag_tree/subtag_tree.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form.html` & `monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page.html` & `monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transactions_table/condensed_row_content.html` & `monopyly-1.3.1/monopyly/templates/credit/transactions_table/condensed_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transactions_table/expanded_row_content.html` & `monopyly-1.3.1/monopyly/templates/credit/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html` & `monopyly-1.3.1/monopyly/templates/credit/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/.gitignore` & `monopyly-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/COPYING` & `monopyly-1.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.0/pyproject.toml` & `monopyly-1.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ['hatchling', 'hatch-vcs', 'hatch-fancy-pypi-readme']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'monopyly'
 authors = [
-    { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
+  { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
 ]
 description = 'A homemade personal finance manager.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.9,<3.11'
 dependencies = [
-    'authanor>=1.0.1',
-    'flask>=2.2.2',
-    'flask-wtf',
-    'markdown>=3.4.3',
-    'python-dateutil',
-    'sqlalchemy>=2.0.0',
+  'authanor>=1.0.2',
+  'flask>=2.2.2',
+  'flask-wtf',
+  'markdown>=3.4.3',
+  'python-dateutil',
+  'sqlalchemy>=2.0.0',
 ]
 keywords = [
   'Finance',
   'Personal Finance',
 ]
 classifiers = [
   'Development Status :: 3 - Alpha',
@@ -73,28 +73,34 @@
 replacement = 'src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/\1"'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/mitchnegus/monopyly/blob/main/\g<2>)'
 
 [tool.pytest.ini_options]
+addopts = [
+  '--import-mode=importlib',
+]
+pythonpath = ["tests/helpers"]
+norecursedirs = ["tests/helpers"]
 filterwarnings = [
-    'ignore::DeprecationWarning',
-    'ignore:INSECURE:UserWarning',
+  'ignore::DeprecationWarning',
+  'ignore:INSECURE:UserWarning',
 ]
 
 [tool.coverage.run]
 omit = [
-    'tests/*',
+  'tests/*',
 ]
 
 [tool.coverage.report]
 exclude_lines = [
-    'raise NotImplementedError',
+  'raise NotImplementedError',
 ]
 
 [tool.black]
 force-exclude = 'monopyly/_version.py'
 
 [tool.isort]
 profile = 'black'
 src_paths = ['monopyly', 'tests']
+known_local_folder = ["test_helpers", "test_tag_helpers"]
```

### Comparing `monopyly-1.3.0/PKG-INFO` & `monopyly-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopyly
-Version: 1.3.0
+Version: 1.3.1
 Summary: A homemade personal finance manager.
 Project-URL: Download, https://pypi.org/project/monopyly
 Project-URL: Homepage, https://github.com/mitchnegus/monopyly
 Project-URL: Repository, https://github.com/mitchnegus/monopyly
 Project-URL: Changelog, https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
@@ -19,15 +19,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Python: <3.11,>=3.9
-Requires-Dist: authanor>=1.0.1
+Requires-Dist: authanor>=1.0.2
 Requires-Dist: flask-wtf
 Requires-Dist: flask>=2.2.2
 Requires-Dist: markdown>=3.4.3
 Requires-Dist: python-dateutil
 Requires-Dist: sqlalchemy>=2.0.0
 Description-Content-Type: text/markdown
```

