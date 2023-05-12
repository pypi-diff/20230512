# Comparing `tmp/fern_belvo-0.0.23.tar.gz` & `tmp/fern_belvo-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_belvo-0.0.23.tar", max compression
+gzip compressed data, was "fern_belvo-0.0.24.tar", max compression
```

## Comparing `fern_belvo-0.0.23.tar` & `fern_belvo-0.0.24.tar`

### file list

```diff
@@ -1,482 +1,482 @@
--rw-r--r--   0        0        0     2578 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/README.md
--rw-r--r--   0        0        0      433 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/pyproject.toml
--rw-r--r--   0        0        0    28390 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/__init__.py
--rw-r--r--   0        0        0    14502 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/client.py
--rw-r--r--   0        0        0      348 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      247 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/environment.py
--rw-r--r--   0        0        0      594 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/__init__.py
--rw-r--r--   0        0        0      346 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/bad_request_error.py
--rw-r--r--   0        0        0      341 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/forbidden_error.py
--rw-r--r--   0        0        0      323 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/internal_server_error.py
--rw-r--r--   0        0        0      325 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/not_found_error.py
--rw-r--r--   0        0        0      340 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/precondition_error.py
--rw-r--r--   0        0        0      349 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/request_timeout_error.py
--rw-r--r--   0        0        0      340 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/py.typed
--rw-r--r--   0        0        0     1252 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/accounts/__init__.py
--rw-r--r--   0        0        0    24733 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/balances/__init__.py
--rw-r--r--   0        0        0    22091 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/balances/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/bank_accounts/__init__.py
--rw-r--r--   0        0        0    12709 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/bank_accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/categorization/__init__.py
--rw-r--r--   0        0        0     5028 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/categorization/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/customers/__init__.py
--rw-r--r--   0        0        0    11113 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/customers/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/employment_records/__init__.py
--rw-r--r--   0        0        0    13705 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/employment_records/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/income_verification/__init__.py
--rw-r--r--   0        0        0     6903 2023-05-12 20:08:15.525380 fern_belvo-0.0.23/src/belvo/resources/income_verification/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/incomes/__init__.py
--rw-r--r--   0        0        0    18173 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/incomes/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/institutions/__init__.py
--rw-r--r--   0        0        0     8625 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/institutions/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/investment_portfolios/__init__.py
--rw-r--r--   0        0        0    18396 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/investment_portfolios/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/invoices/__init__.py
--rw-r--r--   0        0        0    23104 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/invoices/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/links/__init__.py
--rw-r--r--   0        0        0    28442 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/links/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/owners/__init__.py
--rw-r--r--   0        0        0    19537 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/owners/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_institutions/__init__.py
--rw-r--r--   0        0        0     7621 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_institutions/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_intents/__init__.py
--rw-r--r--   0        0        0    16549 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_intents/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_links/__init__.py
--rw-r--r--   0        0        0    12299 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_links/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_transactions/__init__.py
--rw-r--r--   0        0        0    10197 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_transactions/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_webhooks/__init__.py
--rw-r--r--   0        0        0    12533 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/payment_webhooks/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/receivable_transactions/__init__.py
--rw-r--r--   0        0        0    16437 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/receivable_transactions/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/recurring_expenses/__init__.py
--rw-r--r--   0        0        0    19082 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/recurring_expenses/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/risk_insights/__init__.py
--rw-r--r--   0        0        0    18419 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/risk_insights/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/secret_keys/__init__.py
--rw-r--r--   0        0        0     5834 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/secret_keys/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_compliance_status/__init__.py
--rw-r--r--   0        0        0    15080 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_compliance_status/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_declarations/__init__.py
--rw-r--r--   0        0        0    16148 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_declarations/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_retentions/__init__.py
--rw-r--r--   0        0        0    14521 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_retentions/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_returns/__init__.py
--rw-r--r--   0        0        0    16708 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_returns/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_status/__init__.py
--rw-r--r--   0        0        0    14841 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/tax_status/client.py
--rw-r--r--   0        0        0       65 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/transactions/__init__.py
--rw-r--r--   0        0        0    34023 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/resources/transactions/client.py
--rw-r--r--   0        0        0    42168 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/access_to_resource_denied.py
--rw-r--r--   0        0        0     4506 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/account.py
--rw-r--r--   0        0        0     2443 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_balance.py
--rw-r--r--   0        0        0     2241 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_credit_data.py
--rw-r--r--   0        0        0     1594 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_funds_data.py
--rw-r--r--   0        0        0      958 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_funds_data_public_identifications.py
--rw-r--r--   0        0        0     4780 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_loan_data.py
--rw-r--r--   0        0        0      935 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_loan_data_fees.py
--rw-r--r--   0        0        0     1191 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_loan_data_interest_rate.py
--rw-r--r--   0        0        0     1674 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_paginated_response.py
--rw-r--r--   0        0        0     1349 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/accounts_receivables_data.py
--rw-r--r--   0        0        0     1588 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/annual_costs_and_deductions_statement_business.py
--rw-r--r--   0        0        0     1883 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/annual_income_statement_business.py
--rw-r--r--   0        0        0     1282 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/annual_income_statement_individual.py
--rw-r--r--   0        0        0     1514 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/annual_totals_individual.py
--rw-r--r--   0        0        0      992 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/asynchronous_accepted_202.py
--rw-r--r--   0        0        0     1014 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bad_request_error_body_item.py
--rw-r--r--   0        0        0     1827 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/balance.py
--rw-r--r--   0        0        0     1671 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/balances_paginated_response.py
--rw-r--r--   0        0        0     1990 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/balances_request.py
--rw-r--r--   0        0        0     2531 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_business_pse.py
--rw-r--r--   0        0        0     1189 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_details_ofpi.py
--rw-r--r--   0        0        0      930 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_details_ofpi_pix.py
--rw-r--r--   0        0        0     1196 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_details_open_finance.py
--rw-r--r--   0        0        0      937 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_details_open_finance_pix.py
--rw-r--r--   0        0        0     1094 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_holder_request_ofpi.py
--rw-r--r--   0        0        0      356 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_holder_request_ofpi_information.py
--rw-r--r--   0        0        0      966 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_information_content_pse.py
--rw-r--r--   0        0        0     1077 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_information_pse.py
--rw-r--r--   0        0        0     1852 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_ofpi_response.py
--rw-r--r--   0        0        0      309 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_ofpi_response_details.py
--rw-r--r--   0        0        0     1801 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_paginated_response.py
--rw-r--r--   0        0        0      311 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_paginated_response_results_item.py
--rw-r--r--   0        0        0      176 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/bank_account_pse_response.py
--rw-r--r--   0        0        0     1439 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/beneficiary_bank_account_ofpi.py
--rw-r--r--   0        0        0      356 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/beneficiary_bank_account_ofpi_details.py
--rw-r--r--   0        0        0     1242 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/beneficiary_bank_account_pse.py
--rw-r--r--   0        0        0      945 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/categorization.py
--rw-r--r--   0        0        0     3020 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/categorization_body.py
--rw-r--r--   0        0        0     2488 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/categorization_body_request.py
--rw-r--r--   0        0        0     1052 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/categorization_merchant_data.py
--rw-r--r--   0        0        0      848 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/change_access_mode.py
--rw-r--r--   0        0        0     3723 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge.py
--rw-r--r--   0        0        0      342 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details.py
--rw-r--r--   0        0        0      972 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_ofpi.py
--rw-r--r--   0        0        0     1135 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_ofpi_content.py
--rw-r--r--   0        0        0      959 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_pse.py
--rw-r--r--   0        0        0     1127 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_pse_content.py
--rw-r--r--   0        0        0      703 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/charge_status.py
--rw-r--r--   0        0        0     1304 2023-05-12 20:08:15.529380 fern_belvo-0.0.23/src/belvo/types/create_bank_account_ofpi.py
--rw-r--r--   0        0        0      307 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_bank_account_ofpi_details.py
--rw-r--r--   0        0        0     1863 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_bank_account_pse.py
--rw-r--r--   0        0        0      284 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_bank_account_request.py
--rw-r--r--   0        0        0      297 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_bank_account_response.py
--rw-r--r--   0        0        0     1521 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_customer_ofpi.py
--rw-r--r--   0        0        0     1517 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_customer_pse.py
--rw-r--r--   0        0        0      261 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_customer_request.py
--rw-r--r--   0        0        0      224 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_customer_response.py
--rw-r--r--   0        0        0     2638 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_intent_pse.py
--rw-r--r--   0        0        0      134 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_intent_pse_amount.py
--rw-r--r--   0        0        0     2894 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_link_ofpi.py
--rw-r--r--   0        0        0      135 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_link_ofpi_amount.py
--rw-r--r--   0        0        0     2835 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_link_pse.py
--rw-r--r--   0        0        0      132 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_payment_link_pse_amount.py
--rw-r--r--   0        0        0      284 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_paymentlink_request.py
--rw-r--r--   0        0        0      247 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/create_paymentlink_response.py
--rw-r--r--   0        0        0     1855 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/customer_ofpi.py
--rw-r--r--   0        0        0     1784 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/customer_paginated_response.py
--rw-r--r--   0        0        0      238 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/customer_paginated_response_results_item.py
--rw-r--r--   0        0        0     2229 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/customer_pse.py
--rw-r--r--   0        0        0      297 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_bank_account_response.py
--rw-r--r--   0        0        0      253 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_create_paymentlink_response.py
--rw-r--r--   0        0        0      224 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_customer_response.py
--rw-r--r--   0        0        0      237 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_invoice_response.py
--rw-r--r--   0        0        0      301 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_tax_declaration_response.py
--rw-r--r--   0        0        0      450 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_tax_return_response.py
--rw-r--r--   0        0        0      233 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/detail_tax_status_response.py
--rw-r--r--   0        0        0      972 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_confirmation_required_content_pse.py
--rw-r--r--   0        0        0     1301 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_confirmation_required_ofpi.py
--rw-r--r--   0        0        0     1001 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_credentials_required_content_pse.py
--rw-r--r--   0        0        0     1279 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_customer_bank_accounts_content_pse.py
--rw-r--r--   0        0        0      913 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_payment_failed.py
--rw-r--r--   0        0        0     1055 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_payment_method_information_content_ofpi.py
--rw-r--r--   0        0        0     1489 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_payment_method_information_content_pse.py
--rw-r--r--   0        0        0      917 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_payment_processing.py
--rw-r--r--   0        0        0      916 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_payment_succeeded.py
--rw-r--r--   0        0        0      861 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/display_token_required_content_pse.py
--rw-r--r--   0        0        0     1005 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/document_id_business.py
--rw-r--r--   0        0        0     1007 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/document_id_individual.py
--rw-r--r--   0        0        0     1277 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/document_information_business.py
--rw-r--r--   0        0        0     1275 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/document_information_individual.py
--rw-r--r--   0        0        0     2557 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record.py
--rw-r--r--   0        0        0     2769 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_detail.py
--rw-r--r--   0        0        0     1086 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_document_id.py
--rw-r--r--   0        0        0     1317 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_employment_status_updates.py
--rw-r--r--   0        0        0     1584 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_entitlement.py
--rw-r--r--   0        0        0     1034 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_file.py
--rw-r--r--   0        0        0     1843 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_personal_data.py
--rw-r--r--   0        0        0     1353 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_request.py
--rw-r--r--   0        0        0     1495 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_record_social_security_summary.py
--rw-r--r--   0        0        0     1732 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/employment_records_paginated_response.py
--rw-r--r--   0        0        0      123 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_account_category.py
--rw-r--r--   0        0        0      630 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_bank_account_holder_type_ofpi.py
--rw-r--r--   0        0        0      506 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_bank_account_holder_type_pse.py
--rw-r--r--   0        0        0      850 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py
--rw-r--r--   0        0        0     1179 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_categorization_account_category.py
--rw-r--r--   0        0        0      668 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_categorization_account_holder_type.py
--rw-r--r--   0        0        0      141 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_categorization_transaction_category.py
--rw-r--r--   0        0        0      144 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_categorization_transaction_subcategory.py
--rw-r--r--   0        0        0      702 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_categorization_transaction_type.py
--rw-r--r--   0        0        0      592 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_customer_identifier_type_ofpi.py
--rw-r--r--   0        0        0     1031 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_customer_identifier_type_pse.py
--rw-r--r--   0        0        0      699 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_customer_type.py
--rw-r--r--   0        0        0      495 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_employment_record_document_type.py
--rw-r--r--   0        0        0      532 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_employment_record_status.py
--rw-r--r--   0        0        0     1719 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_employment_record_status_update_events.py
--rw-r--r--   0        0        0      911 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_minimum_confidence_level_request.py
--rw-r--r--   0        0        0      475 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_source_type.py
--rw-r--r--   0        0        0      824 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_stream_confidence.py
--rw-r--r--   0        0        0     1495 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_stream_frequency.py
--rw-r--r--   0        0        0     2123 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_stream_type.py
--rw-r--r--   0        0        0      758 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_verification_account_category.py
--rw-r--r--   0        0        0      484 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_verification_account_holder_type.py
--rw-r--r--   0        0        0      359 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_income_verification_type.py
--rw-r--r--   0        0        0      862 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_institution_integration_type.py
--rw-r--r--   0        0        0      630 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_institution_status.py
--rw-r--r--   0        0        0      805 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_institution_type.py
--rw-r--r--   0        0        0     1687 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_investment_portfolio_instrument_type.py
--rw-r--r--   0        0        0     1084 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_investment_portfolio_type.py
--rw-r--r--   0        0        0     2329 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_allowed_income_types_request.py
--rw-r--r--   0        0        0      470 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_dian_invoice_type.py
--rw-r--r--   0        0        0      132 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_dian_payment_method.py
--rw-r--r--   0        0        0      986 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_sat_invoice_type.py
--rw-r--r--   0        0        0      131 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_sat_payment_method.py
--rw-r--r--   0        0        0      119 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_invoice_type.py
--rw-r--r--   0        0        0      923 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_link_access_mode_request.py
--rw-r--r--   0        0        0      130 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_link_access_mode_response.py
--rw-r--r--   0        0        0      123 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_link_refresh_rate.py
--rw-r--r--   0        0        0     1144 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_link_status.py
--rw-r--r--   0        0        0      869 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_loan_data_fee_type.py
--rw-r--r--   0        0        0      513 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_loan_data_interest_rate_type.py
--rw-r--r--   0        0        0      636 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_intent_holder_type_pse.py
--rw-r--r--   0        0        0     1196 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_intent_status.py
--rw-r--r--   0        0        0      728 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_link_allowed_payment_method.py
--rw-r--r--   0        0        0      711 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_link_provider.py
--rw-r--r--   0        0        0      981 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_links_status.py
--rw-r--r--   0        0        0      682 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payment_transaction_type.py
--rw-r--r--   0        0        0      571 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payments_country.py
--rw-r--r--   0        0        0      586 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_payments_currency.py
--rw-r--r--   0        0        0      416 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_receivable_transaction_fee_type.py
--rw-r--r--   0        0        0      930 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_receivable_transaction_status.py
--rw-r--r--   0        0        0      133 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_receivable_transaction_type.py
--rw-r--r--   0        0        0     2023 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_category.py
--rw-r--r--   0        0        0      513 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_frequency.py
--rw-r--r--   0        0        0      552 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_payment_type.py
--rw-r--r--   0        0        0      760 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_tax_compliance_status_outcome.py
--rw-r--r--   0        0        0      526 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_payment_status.py
--rw-r--r--   0        0        0      544 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_receiver_nationality.py
--rw-r--r--   0        0        0      735 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_type.py
--rw-r--r--   0        0        0      129 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_transaction_bill_status.py
--rw-r--r--   0        0        0      127 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_transaction_category.py
--rw-r--r--   0        0        0      125 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_transaction_status.py
--rw-r--r--   0        0        0      130 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_transaction_subcategory.py
--rw-r--r--   0        0        0      123 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/enum_transaction_type.py
--rw-r--r--   0        0        0     2117 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/equity_statement_business.py
--rw-r--r--   0        0        0     1137 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/equity_statement_individual.py
--rw-r--r--   0        0        0     2410 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/eyod_income_verification_body_request.py
--rw-r--r--   0        0        0     1525 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/gross_income_individual.py
--rw-r--r--   0        0        0     1067 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_bank_account_information_pse.py
--rw-r--r--   0        0        0     1089 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_bank_account_pse.py
--rw-r--r--   0        0        0     1045 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_business_pse.py
--rw-r--r--   0        0        0     1179 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_business_response_pse.py
--rw-r--r--   0        0        0     1189 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_business_ofpi.py
--rw-r--r--   0        0        0     1073 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_business_ofpi_response.py
--rw-r--r--   0        0        0      935 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_business_pse.py
--rw-r--r--   0        0        0      993 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_business_pse_response.py
--rw-r--r--   0        0        0     1290 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_individual_ofpi.py
--rw-r--r--   0        0        0     1174 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_information_individual_ofpi_response.py
--rw-r--r--   0        0        0     1043 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_response_ofpi.py
--rw-r--r--   0        0        0      402 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/holder_response_ofpi_information.py
--rw-r--r--   0        0        0     4077 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/income.py
--rw-r--r--   0        0        0     4769 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/income_streams_body.py
--rw-r--r--   0        0        0     1666 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/incomes_paginated_response.py
--rw-r--r--   0        0        0     2630 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/incomes_request.py
--rw-r--r--   0        0        0     3940 2023-05-12 20:08:15.533381 fern_belvo-0.0.23/src/belvo/types/institution.py
--rw-r--r--   0        0        0     1205 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institution_account.py
--rw-r--r--   0        0        0     1992 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institution_down_error.py
--rw-r--r--   0        0        0     2062 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institution_form_field.py
--rw-r--r--   0        0        0     1897 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institution_inactive_error.py
--rw-r--r--   0        0        0     2013 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institution_unavailable_error.py
--rw-r--r--   0        0        0      937 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institutions_feature.py
--rw-r--r--   0        0        0     1937 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institutions_form_field.py
--rw-r--r--   0        0        0     1513 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institutions_form_field_values.py
--rw-r--r--   0        0        0     1691 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/institutions_paginated_response.py
--rw-r--r--   0        0        0     2005 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invalid_access_mode.py
--rw-r--r--   0        0        0     1939 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invalid_link_error.py
--rw-r--r--   0        0        0     1970 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invalid_period_error.py
--rw-r--r--   0        0        0     2666 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio.py
--rw-r--r--   0        0        0     4088 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument.py
--rw-r--r--   0        0        0     1056 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_fees.py
--rw-r--r--   0        0        0     1465 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_interest_rate.py
--rw-r--r--   0        0        0     1008 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_public_id.py
--rw-r--r--   0        0        0      952 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py
--rw-r--r--   0        0        0     1751 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/investments_portfolios_paginated_response.py
--rw-r--r--   0        0        0     2518 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_detail_dian.py
--rw-r--r--   0        0        0     1418 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_detail_retained_tax_sat.py
--rw-r--r--   0        0        0     3179 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_detail_sat.py
--rw-r--r--   0        0        0     7894 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_dian.py
--rw-r--r--   0        0        0     2328 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_sender_details_dian.py
--rw-r--r--   0        0        0     1066 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_warnings_dian.py
--rw-r--r--   0        0        0      925 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_warnings_sat.py
--rw-r--r--   0        0        0     9762 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoice_with_id_sat.py
--rw-r--r--   0        0        0     2919 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payments_dian.py
--rw-r--r--   0        0        0     2063 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payments_related_documents_dian.py
--rw-r--r--   0        0        0     2030 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payments_related_documents_sat.py
--rw-r--r--   0        0        0     3037 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payments_sat.py
--rw-r--r--   0        0        0     2066 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payroll_dian.py
--rw-r--r--   0        0        0     1782 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_payroll_sat.py
--rw-r--r--   0        0        0     2345 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_receiver_details_dian.py
--rw-r--r--   0        0        0     2061 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_request.py
--rw-r--r--   0        0        0     1809 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_response_paginated_response.py
--rw-r--r--   0        0        0      260 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/invoices_response_paginated_response_results_item.py
--rw-r--r--   0        0        0     1249 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_invalid_credentials.py
--rw-r--r--   0        0        0     1227 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_invalid_token.py
--rw-r--r--   0        0        0     1257 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_login_error.py
--rw-r--r--   0        0        0     1243 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_payment_error.py
--rw-r--r--   0        0        0     1289 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_session_expired.py
--rw-r--r--   0        0        0     1261 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/last_error_two_factor.py
--rw-r--r--   0        0        0     2833 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/link.py
--rw-r--r--   0        0        0     4669 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/links_put_request.py
--rw-r--r--   0        0        0     7955 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/links_request.py
--rw-r--r--   0        0        0      554 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/list_payment_links_request_ordering.py
--rw-r--r--   0        0        0      521 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/list_payment_links_request_status.py
--rw-r--r--   0        0        0      356 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/list_tax_declarations_response.py
--rw-r--r--   0        0        0      586 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/list_tax_returns_response.py
--rw-r--r--   0        0        0     2700 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/login_error.py
--rw-r--r--   0        0        0      913 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/needs_redirect_content.py
--rw-r--r--   0        0        0      923 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/needs_redirect_content_pse.py
--rw-r--r--   0        0        0     1588 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/net_income_individual.py
--rw-r--r--   0        0        0     1661 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_ofpi.py
--rw-r--r--   0        0        0     2256 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py
--rw-r--r--   0        0        0     1674 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_pse.py
--rw-r--r--   0        0        0     2850 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_pse_type.py
--rw-r--r--   0        0        0     1666 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_credentials_required_pse.py
--rw-r--r--   0        0        0     2840 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_credentials_required_pse_type.py
--rw-r--r--   0        0        0     1677 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_customer_bank_accounts_pse.py
--rw-r--r--   0        0        0     2850 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py
--rw-r--r--   0        0        0     1596 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_needs_redirect_pse.py
--rw-r--r--   0        0        0     2780 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_needs_redirect_pse_type.py
--rw-r--r--   0        0        0     1574 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_failed.py
--rw-r--r--   0        0        0     2179 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_failed_type.py
--rw-r--r--   0        0        0     1701 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information.py
--rw-r--r--   0        0        0     1875 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_pse.py
--rw-r--r--   0        0        0     2890 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_pse_type.py
--rw-r--r--   0        0        0     2256 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_type.py
--rw-r--r--   0        0        0     1607 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_processing.py
--rw-r--r--   0        0        0     2207 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_processing_type.py
--rw-r--r--   0        0        0     1599 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_succeeded.py
--rw-r--r--   0        0        0     2200 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_succeeded_type.py
--rw-r--r--   0        0        0     2131 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_token_required_pse.py
--rw-r--r--   0        0        0     2780 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_display_token_required_pse_type.py
--rw-r--r--   0        0        0     1546 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_needs_redirect.py
--rw-r--r--   0        0        0     2130 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/next_step_needs_redirect_type.py
--rw-r--r--   0        0        0     1531 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/non_taxable_income_individual.py
--rw-r--r--   0        0        0     1706 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/not_found_error_body.py
--rw-r--r--   0        0        0     2545 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/owner.py
--rw-r--r--   0        0        0     1584 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/owner_document_id.py
--rw-r--r--   0        0        0     1661 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/owners_paginated_response.py
--rw-r--r--   0        0        0     1596 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/paginated_response_link.py
--rw-r--r--   0        0        0     1798 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/patch_body.py
--rw-r--r--   0        0        0     1479 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/patch_body_without_save_data.py
--rw-r--r--   0        0        0      241 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/patch_invoices_response_item.py
--rw-r--r--   0        0        0      876 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/patch_payment_intents_body_pse.py
--rw-r--r--   0        0        0     2677 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/patch_payment_method_details_pse.py
--rw-r--r--   0        0        0     2302 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_institution.py
--rw-r--r--   0        0        0     4025 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_ofpi.py
--rw-r--r--   0        0        0      846 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_ofpi_next_step.py
--rw-r--r--   0        0        0      462 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_ofpi_payment_method_details.py
--rw-r--r--   0        0        0     1733 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_paginated_response.py
--rw-r--r--   0        0        0     1549 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py
--rw-r--r--   0        0        0     1551 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py
--rw-r--r--   0        0        0     2222 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_pse.py
--rw-r--r--   0        0        0     1013 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py
--rw-r--r--   0        0        0     1030 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py
--rw-r--r--   0        0        0      983 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_pse.py
--rw-r--r--   0        0        0     4050 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_pse.py
--rw-r--r--   0        0        0      656 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_pse_last_error.py
--rw-r--r--   0        0        0      933 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intent_pse_next_step.py
--rw-r--r--   0        0        0     1644 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intents_payment_method_details_body_pse.py
--rw-r--r--   0        0        0      995 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_intents_payment_method_details_pse.py
--rw-r--r--   0        0        0     1499 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_callback_urls.py
--rw-r--r--   0        0        0     1408 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_callback_urls_response.py
--rw-r--r--   0        0        0     2547 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_list_ofpi.py
--rw-r--r--   0        0        0     2546 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_list_pse.py
--rw-r--r--   0        0        0     2331 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_ofpi.py
--rw-r--r--   0        0        0     1801 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_paginated_response.py
--rw-r--r--   0        0        0      287 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_paginated_response_results_item.py
--rw-r--r--   0        0        0     2326 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_link_pse.py
--rw-r--r--   0        0        0     1244 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_links_payment_method_details_body_ofpi.py
--rw-r--r--   0        0        0     1646 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_links_payment_method_details_body_pse.py
--rw-r--r--   0        0        0     1021 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_details_ofpi.py
--rw-r--r--   0        0        0      980 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_details_pse.py
--rw-r--r--   0        0        0     1530 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py
--rw-r--r--   0        0        0     1256 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_information_body_ofpi.py
--rw-r--r--   0        0        0     1390 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_information_body_pse.py
--rw-r--r--   0        0        0     1013 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_information_details_pse.py
--rw-r--r--   0        0        0      967 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_information_ofpi.py
--rw-r--r--   0        0        0     1043 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_method_information_pse.py
--rw-r--r--   0        0        0     2247 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_transaction.py
--rw-r--r--   0        0        0      313 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_transaction_payer.py
--rw-r--r--   0        0        0     1527 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payment_webhook.py
--rw-r--r--   0        0        0     1742 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payments_institutions_paginated_response.py
--rw-r--r--   0        0        0     1742 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payments_transactions_paginated_response.py
--rw-r--r--   0        0        0     1471 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payments_way.py
--rw-r--r--   0        0        0     1708 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/payments_webhooks_paginated_response.py
--rw-r--r--   0        0        0     1072 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/pension_income_statement_individual.py
--rw-r--r--   0        0        0      817 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/providers_pse.py
--rw-r--r--   0        0        0     1866 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/receivable_transaction_request.py
--rw-r--r--   0        0        0     2957 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/receivables_transaction.py
--rw-r--r--   0        0        0     1042 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/receivables_transaction_account.py
--rw-r--r--   0        0        0     1065 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/receivables_transaction_number_of_installments.py
--rw-r--r--   0        0        0     1750 2023-05-12 20:08:15.537381 fern_belvo-0.0.23/src/belvo/types/receivables_transactions_paginated_response.py
--rw-r--r--   0        0        0     1026 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/recevables_transaction_fees.py
--rw-r--r--   0        0        0     1242 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/recurring_expense_source_transaction.py
--rw-r--r--   0        0        0     2895 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/recurring_expenses.py
--rw-r--r--   0        0        0     1735 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/recurring_expenses_paginated_response.py
--rw-r--r--   0        0        0     2148 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/recurring_expenses_request.py
--rw-r--r--   0        0        0     1120 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/reporting_id.py
--rw-r--r--   0        0        0     2054 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/request_timeout_error_body.py
--rw-r--r--   0        0        0     1454 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retention_breakdown.py
--rw-r--r--   0        0        0      244 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retrieve_invoices_response_item.py
--rw-r--r--   0        0        0      308 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retrieve_tax_declarations_response_item.py
--rw-r--r--   0        0        0      307 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retrieve_tax_returns_request_body.py
--rw-r--r--   0        0        0      457 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retrieve_tax_returns_response_item.py
--rw-r--r--   0        0        0      235 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/retrieve_tax_status_response.py
--rw-r--r--   0        0        0     1980 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights.py
--rw-r--r--   0        0        0     3951 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_balance_metrics.py
--rw-r--r--   0        0        0     3942 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_cashflow_metrics.py
--rw-r--r--   0        0        0     1093 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_credit_card_metrics.py
--rw-r--r--   0        0        0     1369 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_loans_metrics.py
--rw-r--r--   0        0        0     1711 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_paginated_response.py
--rw-r--r--   0        0        0     9169 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/risk_insights_transaction_metrics.py
--rw-r--r--   0        0        0     1176 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/secret_keys.py
--rw-r--r--   0        0        0     1694 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/secret_keys_paginated_response.py
--rw-r--r--   0        0        0     2016 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/session_expired_error.py
--rw-r--r--   0        0        0     1276 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/standard_request.py
--rw-r--r--   0        0        0     2491 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_assessment_business.py
--rw-r--r--   0        0        0     2771 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_assessment_individual.py
--rw-r--r--   0        0        0     1788 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_compliance_status.py
--rw-r--r--   0        0        0     1748 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_compliance_status_paginated_response.py
--rw-r--r--   0        0        0     1326 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_compliance_status_request.py
--rw-r--r--   0        0        0     2291 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_declaration_business.py
--rw-r--r--   0        0        0     1755 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_declaration_business_paginated.py
--rw-r--r--   0        0        0     2281 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_declaration_individual.py
--rw-r--r--   0        0        0     1765 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_declaration_individual_paginated.py
--rw-r--r--   0        0        0     1727 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_declarations_request.py
--rw-r--r--   0        0        0     1666 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_payer_information_business.py
--rw-r--r--   0        0        0     1489 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_payer_information_individual.py
--rw-r--r--   0        0        0     3880 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_retentions.py
--rw-r--r--   0        0        0     1716 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_retentions_paginated_response.py
--rw-r--r--   0        0        0     1989 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_retentions_request.py
--rw-r--r--   0        0        0      129 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_return_business.py
--rw-r--r--   0        0        0      136 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_return_business_monthly.py
--rw-r--r--   0        0        0      129 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_return_personal.py
--rw-r--r--   0        0        0      136 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_return_personal_monthly.py
--rw-r--r--   0        0        0      146 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_business_monthly_paginated.py
--rw-r--r--   0        0        0      139 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_business_paginated.py
--rw-r--r--   0        0        0     2175 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_monthly_request.py
--rw-r--r--   0        0        0      146 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_personal_monthly_paginated.py
--rw-r--r--   0        0        0      139 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_personal_paginated.py
--rw-r--r--   0        0        0     1967 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_returns_yearly_request.py
--rw-r--r--   0        0        0     1089 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_address_between_street_dian.py
--rw-r--r--   0        0        0     1029 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_address_between_street_sat.py
--rw-r--r--   0        0        0     2076 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_address_dian.py
--rw-r--r--   0        0        0     1919 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_address_sat.py
--rw-r--r--   0        0        0     3269 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_dian.py
--rw-r--r--   0        0        0     1728 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_economic_activity_dian.py
--rw-r--r--   0        0        0     1328 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_economic_activity_sat.py
--rw-r--r--   0        0        0     1550 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_obligations_dian.py
--rw-r--r--   0        0        0     1357 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_obligations_sat.py
--rw-r--r--   0        0        0     1784 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_paginated_response.py
--rw-r--r--   0        0        0      247 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_paginated_response_results_item.py
--rw-r--r--   0        0        0     1179 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_regimens_dian.py
--rw-r--r--   0        0        0     1048 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_regimens_sat.py
--rw-r--r--   0        0        0     1316 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_request.py
--rw-r--r--   0        0        0     3194 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_sat.py
--rw-r--r--   0        0        0     2648 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_tax_payer_information_dian.py
--rw-r--r--   0        0        0     2672 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/tax_status_tax_payer_information_sat.py
--rw-r--r--   0        0        0     2431 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/token_required_response.py
--rw-r--r--   0        0        0     1605 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/token_required_response_token_generation_data.py
--rw-r--r--   0        0        0     2136 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/too_many_sessions_error.py
--rw-r--r--   0        0        0     3391 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction.py
--rw-r--r--   0        0        0     1052 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction_bank_account_body_pse.py
--rw-r--r--   0        0        0      138 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction_bank_account_ofpi.py
--rw-r--r--   0        0        0      325 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction_bank_account_pse.py
--rw-r--r--   0        0        0     1689 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction_credit_card_data.py
--rw-r--r--   0        0        0     1049 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transaction_merchant_data.py
--rw-r--r--   0        0        0     1691 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transactions_paginated_response.py
--rw-r--r--   0        0        0     2001 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/transactions_request.py
--rw-r--r--   0        0        0     1946 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     2080 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/unconfirmed_link_error.py
--rw-r--r--   0        0        0     2016 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/unexpected_error.py
--rw-r--r--   0        0        0     2035 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/unsupported_operation_error.py
--rw-r--r--   0        0        0     2660 2023-05-12 20:08:15.541381 fern_belvo-0.0.23/src/belvo/types/validation_error.py
--rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 fern_belvo-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0     2578 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/README.md
+-rw-r--r--   0        0        0      433 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0    28390 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/__init__.py
+-rw-r--r--   0        0        0    16332 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/client.py
+-rw-r--r--   0        0        0      348 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      247 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/environment.py
+-rw-r--r--   0        0        0      594 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/bad_request_error.py
+-rw-r--r--   0        0        0      341 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/forbidden_error.py
+-rw-r--r--   0        0        0      323 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/internal_server_error.py
+-rw-r--r--   0        0        0      325 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/not_found_error.py
+-rw-r--r--   0        0        0      340 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/precondition_error.py
+-rw-r--r--   0        0        0      349 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/request_timeout_error.py
+-rw-r--r--   0        0        0      340 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/py.typed
+-rw-r--r--   0        0        0     1252 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    24969 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/balances/__init__.py
+-rw-r--r--   0        0        0    22327 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/balances/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/bank_accounts/__init__.py
+-rw-r--r--   0        0        0    12881 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/bank_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/categorization/__init__.py
+-rw-r--r--   0        0        0     5136 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/categorization/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/customers/__init__.py
+-rw-r--r--   0        0        0    11285 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/customers/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.703496 fern_belvo-0.0.24/src/belvo/resources/employment_records/__init__.py
+-rw-r--r--   0        0        0    13909 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/employment_records/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/income_verification/__init__.py
+-rw-r--r--   0        0        0     7011 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/income_verification/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/incomes/__init__.py
+-rw-r--r--   0        0        0    18409 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/incomes/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/institutions/__init__.py
+-rw-r--r--   0        0        0     8765 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/institutions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/investment_portfolios/__init__.py
+-rw-r--r--   0        0        0    18632 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/investment_portfolios/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/invoices/__init__.py
+-rw-r--r--   0        0        0    23340 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/invoices/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/links/__init__.py
+-rw-r--r--   0        0        0    28742 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/links/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/owners/__init__.py
+-rw-r--r--   0        0        0    19773 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/owners/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_institutions/__init__.py
+-rw-r--r--   0        0        0     7761 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_institutions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_intents/__init__.py
+-rw-r--r--   0        0        0    16753 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_intents/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_links/__init__.py
+-rw-r--r--   0        0        0    12471 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_links/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_transactions/__init__.py
+-rw-r--r--   0        0        0    10337 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_transactions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_webhooks/__init__.py
+-rw-r--r--   0        0        0    12737 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/payment_webhooks/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/receivable_transactions/__init__.py
+-rw-r--r--   0        0        0    16641 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/receivable_transactions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/recurring_expenses/__init__.py
+-rw-r--r--   0        0        0    19318 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/recurring_expenses/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/risk_insights/__init__.py
+-rw-r--r--   0        0        0    18655 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/risk_insights/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/secret_keys/__init__.py
+-rw-r--r--   0        0        0     5974 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/secret_keys/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_compliance_status/__init__.py
+-rw-r--r--   0        0        0    15284 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_compliance_status/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_declarations/__init__.py
+-rw-r--r--   0        0        0    16352 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_declarations/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_retentions/__init__.py
+-rw-r--r--   0        0        0    14725 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_retentions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_returns/__init__.py
+-rw-r--r--   0        0        0    16912 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_returns/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_status/__init__.py
+-rw-r--r--   0        0        0    15045 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/tax_status/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    34291 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/resources/transactions/client.py
+-rw-r--r--   0        0        0    42168 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/access_to_resource_denied.py
+-rw-r--r--   0        0        0     4506 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/account.py
+-rw-r--r--   0        0        0     2443 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_balance.py
+-rw-r--r--   0        0        0     2241 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_credit_data.py
+-rw-r--r--   0        0        0     1594 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_funds_data.py
+-rw-r--r--   0        0        0      958 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_funds_data_public_identifications.py
+-rw-r--r--   0        0        0     4780 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_loan_data.py
+-rw-r--r--   0        0        0      935 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_loan_data_fees.py
+-rw-r--r--   0        0        0     1191 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_loan_data_interest_rate.py
+-rw-r--r--   0        0        0     1674 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_paginated_response.py
+-rw-r--r--   0        0        0     1349 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/accounts_receivables_data.py
+-rw-r--r--   0        0        0     1588 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/annual_costs_and_deductions_statement_business.py
+-rw-r--r--   0        0        0     1883 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/annual_income_statement_business.py
+-rw-r--r--   0        0        0     1282 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/annual_income_statement_individual.py
+-rw-r--r--   0        0        0     1514 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/annual_totals_individual.py
+-rw-r--r--   0        0        0      992 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/asynchronous_accepted_202.py
+-rw-r--r--   0        0        0     1014 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bad_request_error_body_item.py
+-rw-r--r--   0        0        0     1827 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/balance.py
+-rw-r--r--   0        0        0     1671 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/balances_paginated_response.py
+-rw-r--r--   0        0        0     1990 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/balances_request.py
+-rw-r--r--   0        0        0     2531 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_business_pse.py
+-rw-r--r--   0        0        0     1189 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_details_ofpi.py
+-rw-r--r--   0        0        0      930 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_details_ofpi_pix.py
+-rw-r--r--   0        0        0     1196 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_details_open_finance.py
+-rw-r--r--   0        0        0      937 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_details_open_finance_pix.py
+-rw-r--r--   0        0        0     1094 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_holder_request_ofpi.py
+-rw-r--r--   0        0        0      356 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_holder_request_ofpi_information.py
+-rw-r--r--   0        0        0      966 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_information_content_pse.py
+-rw-r--r--   0        0        0     1077 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_information_pse.py
+-rw-r--r--   0        0        0     1852 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_ofpi_response.py
+-rw-r--r--   0        0        0      309 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_ofpi_response_details.py
+-rw-r--r--   0        0        0     1801 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_paginated_response.py
+-rw-r--r--   0        0        0      311 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_paginated_response_results_item.py
+-rw-r--r--   0        0        0      176 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/bank_account_pse_response.py
+-rw-r--r--   0        0        0     1439 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/beneficiary_bank_account_ofpi.py
+-rw-r--r--   0        0        0      356 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/beneficiary_bank_account_ofpi_details.py
+-rw-r--r--   0        0        0     1242 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/beneficiary_bank_account_pse.py
+-rw-r--r--   0        0        0      945 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/categorization.py
+-rw-r--r--   0        0        0     3020 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/categorization_body.py
+-rw-r--r--   0        0        0     2488 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/categorization_body_request.py
+-rw-r--r--   0        0        0     1052 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/categorization_merchant_data.py
+-rw-r--r--   0        0        0      848 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/change_access_mode.py
+-rw-r--r--   0        0        0     3723 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge.py
+-rw-r--r--   0        0        0      342 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details.py
+-rw-r--r--   0        0        0      972 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_ofpi.py
+-rw-r--r--   0        0        0     1135 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_ofpi_content.py
+-rw-r--r--   0        0        0      959 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_pse.py
+-rw-r--r--   0        0        0     1127 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_pse_content.py
+-rw-r--r--   0        0        0      703 2023-05-12 20:16:51.707496 fern_belvo-0.0.24/src/belvo/types/charge_status.py
+-rw-r--r--   0        0        0     1304 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_bank_account_ofpi.py
+-rw-r--r--   0        0        0      307 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_bank_account_ofpi_details.py
+-rw-r--r--   0        0        0     1863 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_bank_account_pse.py
+-rw-r--r--   0        0        0      284 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_bank_account_request.py
+-rw-r--r--   0        0        0      297 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_bank_account_response.py
+-rw-r--r--   0        0        0     1521 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_customer_ofpi.py
+-rw-r--r--   0        0        0     1517 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_customer_pse.py
+-rw-r--r--   0        0        0      261 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_customer_request.py
+-rw-r--r--   0        0        0      224 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_customer_response.py
+-rw-r--r--   0        0        0     2638 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_intent_pse.py
+-rw-r--r--   0        0        0      134 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_intent_pse_amount.py
+-rw-r--r--   0        0        0     2894 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_link_ofpi.py
+-rw-r--r--   0        0        0      135 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_link_ofpi_amount.py
+-rw-r--r--   0        0        0     2835 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_link_pse.py
+-rw-r--r--   0        0        0      132 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_payment_link_pse_amount.py
+-rw-r--r--   0        0        0      284 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_paymentlink_request.py
+-rw-r--r--   0        0        0      247 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/create_paymentlink_response.py
+-rw-r--r--   0        0        0     1855 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/customer_ofpi.py
+-rw-r--r--   0        0        0     1784 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/customer_paginated_response.py
+-rw-r--r--   0        0        0      238 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/customer_paginated_response_results_item.py
+-rw-r--r--   0        0        0     2229 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/customer_pse.py
+-rw-r--r--   0        0        0      297 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_bank_account_response.py
+-rw-r--r--   0        0        0      253 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_create_paymentlink_response.py
+-rw-r--r--   0        0        0      224 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_customer_response.py
+-rw-r--r--   0        0        0      237 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_invoice_response.py
+-rw-r--r--   0        0        0      301 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_tax_declaration_response.py
+-rw-r--r--   0        0        0      450 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_tax_return_response.py
+-rw-r--r--   0        0        0      233 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/detail_tax_status_response.py
+-rw-r--r--   0        0        0      972 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_confirmation_required_content_pse.py
+-rw-r--r--   0        0        0     1301 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_confirmation_required_ofpi.py
+-rw-r--r--   0        0        0     1001 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_credentials_required_content_pse.py
+-rw-r--r--   0        0        0     1279 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_customer_bank_accounts_content_pse.py
+-rw-r--r--   0        0        0      913 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_payment_failed.py
+-rw-r--r--   0        0        0     1055 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_payment_method_information_content_ofpi.py
+-rw-r--r--   0        0        0     1489 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_payment_method_information_content_pse.py
+-rw-r--r--   0        0        0      917 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_payment_processing.py
+-rw-r--r--   0        0        0      916 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_payment_succeeded.py
+-rw-r--r--   0        0        0      861 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/display_token_required_content_pse.py
+-rw-r--r--   0        0        0     1005 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/document_id_business.py
+-rw-r--r--   0        0        0     1007 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/document_id_individual.py
+-rw-r--r--   0        0        0     1277 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/document_information_business.py
+-rw-r--r--   0        0        0     1275 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/document_information_individual.py
+-rw-r--r--   0        0        0     2557 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record.py
+-rw-r--r--   0        0        0     2769 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_detail.py
+-rw-r--r--   0        0        0     1086 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_document_id.py
+-rw-r--r--   0        0        0     1317 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_employment_status_updates.py
+-rw-r--r--   0        0        0     1584 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_entitlement.py
+-rw-r--r--   0        0        0     1034 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_file.py
+-rw-r--r--   0        0        0     1843 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_personal_data.py
+-rw-r--r--   0        0        0     1353 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_request.py
+-rw-r--r--   0        0        0     1495 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_record_social_security_summary.py
+-rw-r--r--   0        0        0     1732 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/employment_records_paginated_response.py
+-rw-r--r--   0        0        0      123 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_account_category.py
+-rw-r--r--   0        0        0      630 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_bank_account_holder_type_ofpi.py
+-rw-r--r--   0        0        0      506 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_bank_account_holder_type_pse.py
+-rw-r--r--   0        0        0      850 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py
+-rw-r--r--   0        0        0     1179 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_categorization_account_category.py
+-rw-r--r--   0        0        0      668 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_categorization_account_holder_type.py
+-rw-r--r--   0        0        0      141 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_categorization_transaction_category.py
+-rw-r--r--   0        0        0      144 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_categorization_transaction_subcategory.py
+-rw-r--r--   0        0        0      702 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_categorization_transaction_type.py
+-rw-r--r--   0        0        0      592 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_customer_identifier_type_ofpi.py
+-rw-r--r--   0        0        0     1031 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_customer_identifier_type_pse.py
+-rw-r--r--   0        0        0      699 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_customer_type.py
+-rw-r--r--   0        0        0      495 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_employment_record_document_type.py
+-rw-r--r--   0        0        0      532 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_employment_record_status.py
+-rw-r--r--   0        0        0     1719 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_employment_record_status_update_events.py
+-rw-r--r--   0        0        0      911 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_minimum_confidence_level_request.py
+-rw-r--r--   0        0        0      475 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_source_type.py
+-rw-r--r--   0        0        0      824 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_stream_confidence.py
+-rw-r--r--   0        0        0     1495 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_stream_frequency.py
+-rw-r--r--   0        0        0     2123 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_stream_type.py
+-rw-r--r--   0        0        0      758 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_verification_account_category.py
+-rw-r--r--   0        0        0      484 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_verification_account_holder_type.py
+-rw-r--r--   0        0        0      359 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_income_verification_type.py
+-rw-r--r--   0        0        0      862 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_institution_integration_type.py
+-rw-r--r--   0        0        0      630 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_institution_status.py
+-rw-r--r--   0        0        0      805 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_institution_type.py
+-rw-r--r--   0        0        0     1687 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_investment_portfolio_instrument_type.py
+-rw-r--r--   0        0        0     1084 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_investment_portfolio_type.py
+-rw-r--r--   0        0        0     2329 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_allowed_income_types_request.py
+-rw-r--r--   0        0        0      470 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_dian_invoice_type.py
+-rw-r--r--   0        0        0      132 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_dian_payment_method.py
+-rw-r--r--   0        0        0      986 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_sat_invoice_type.py
+-rw-r--r--   0        0        0      131 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_sat_payment_method.py
+-rw-r--r--   0        0        0      119 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_invoice_type.py
+-rw-r--r--   0        0        0      923 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_link_access_mode_request.py
+-rw-r--r--   0        0        0      130 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_link_access_mode_response.py
+-rw-r--r--   0        0        0      123 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_link_refresh_rate.py
+-rw-r--r--   0        0        0     1144 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_link_status.py
+-rw-r--r--   0        0        0      869 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_loan_data_fee_type.py
+-rw-r--r--   0        0        0      513 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_loan_data_interest_rate_type.py
+-rw-r--r--   0        0        0      636 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_intent_holder_type_pse.py
+-rw-r--r--   0        0        0     1196 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_intent_status.py
+-rw-r--r--   0        0        0      728 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_link_allowed_payment_method.py
+-rw-r--r--   0        0        0      711 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_link_provider.py
+-rw-r--r--   0        0        0      981 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_links_status.py
+-rw-r--r--   0        0        0      682 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payment_transaction_type.py
+-rw-r--r--   0        0        0      571 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payments_country.py
+-rw-r--r--   0        0        0      586 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_payments_currency.py
+-rw-r--r--   0        0        0      416 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_receivable_transaction_fee_type.py
+-rw-r--r--   0        0        0      930 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_receivable_transaction_status.py
+-rw-r--r--   0        0        0      133 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_receivable_transaction_type.py
+-rw-r--r--   0        0        0     2023 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_category.py
+-rw-r--r--   0        0        0      513 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_frequency.py
+-rw-r--r--   0        0        0      552 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_payment_type.py
+-rw-r--r--   0        0        0      760 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_tax_compliance_status_outcome.py
+-rw-r--r--   0        0        0      526 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_payment_status.py
+-rw-r--r--   0        0        0      544 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_receiver_nationality.py
+-rw-r--r--   0        0        0      735 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_type.py
+-rw-r--r--   0        0        0      129 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_transaction_bill_status.py
+-rw-r--r--   0        0        0      127 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_transaction_category.py
+-rw-r--r--   0        0        0      125 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_transaction_status.py
+-rw-r--r--   0        0        0      130 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_transaction_subcategory.py
+-rw-r--r--   0        0        0      123 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/enum_transaction_type.py
+-rw-r--r--   0        0        0     2117 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/equity_statement_business.py
+-rw-r--r--   0        0        0     1137 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/equity_statement_individual.py
+-rw-r--r--   0        0        0     2410 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/eyod_income_verification_body_request.py
+-rw-r--r--   0        0        0     1525 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/gross_income_individual.py
+-rw-r--r--   0        0        0     1067 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_bank_account_information_pse.py
+-rw-r--r--   0        0        0     1089 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_bank_account_pse.py
+-rw-r--r--   0        0        0     1045 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_business_pse.py
+-rw-r--r--   0        0        0     1179 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_business_response_pse.py
+-rw-r--r--   0        0        0     1189 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_business_ofpi.py
+-rw-r--r--   0        0        0     1073 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_business_ofpi_response.py
+-rw-r--r--   0        0        0      935 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_business_pse.py
+-rw-r--r--   0        0        0      993 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_business_pse_response.py
+-rw-r--r--   0        0        0     1290 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_individual_ofpi.py
+-rw-r--r--   0        0        0     1174 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_information_individual_ofpi_response.py
+-rw-r--r--   0        0        0     1043 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_response_ofpi.py
+-rw-r--r--   0        0        0      402 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/holder_response_ofpi_information.py
+-rw-r--r--   0        0        0     4077 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/income.py
+-rw-r--r--   0        0        0     4769 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/income_streams_body.py
+-rw-r--r--   0        0        0     1666 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/incomes_paginated_response.py
+-rw-r--r--   0        0        0     2630 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/incomes_request.py
+-rw-r--r--   0        0        0     3939 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/institution.py
+-rw-r--r--   0        0        0     1205 2023-05-12 20:16:51.711496 fern_belvo-0.0.24/src/belvo/types/institution_account.py
+-rw-r--r--   0        0        0     1989 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institution_down_error.py
+-rw-r--r--   0        0        0     2062 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institution_form_field.py
+-rw-r--r--   0        0        0     1894 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institution_inactive_error.py
+-rw-r--r--   0        0        0     2011 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institution_unavailable_error.py
+-rw-r--r--   0        0        0      937 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institutions_feature.py
+-rw-r--r--   0        0        0     1937 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institutions_form_field.py
+-rw-r--r--   0        0        0     1513 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institutions_form_field_values.py
+-rw-r--r--   0        0        0     1691 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/institutions_paginated_response.py
+-rw-r--r--   0        0        0     2002 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invalid_access_mode.py
+-rw-r--r--   0        0        0     1936 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invalid_link_error.py
+-rw-r--r--   0        0        0     1967 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invalid_period_error.py
+-rw-r--r--   0        0        0     2666 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio.py
+-rw-r--r--   0        0        0     4088 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument.py
+-rw-r--r--   0        0        0     1056 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_fees.py
+-rw-r--r--   0        0        0     1465 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_interest_rate.py
+-rw-r--r--   0        0        0     1008 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_public_id.py
+-rw-r--r--   0        0        0      952 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py
+-rw-r--r--   0        0        0     1751 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/investments_portfolios_paginated_response.py
+-rw-r--r--   0        0        0     2518 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_detail_dian.py
+-rw-r--r--   0        0        0     1418 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_detail_retained_tax_sat.py
+-rw-r--r--   0        0        0     3178 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_detail_sat.py
+-rw-r--r--   0        0        0     7893 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_dian.py
+-rw-r--r--   0        0        0     2326 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_sender_details_dian.py
+-rw-r--r--   0        0        0     1066 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_warnings_dian.py
+-rw-r--r--   0        0        0      925 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_warnings_sat.py
+-rw-r--r--   0        0        0     9760 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoice_with_id_sat.py
+-rw-r--r--   0        0        0     2919 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payments_dian.py
+-rw-r--r--   0        0        0     2063 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payments_related_documents_dian.py
+-rw-r--r--   0        0        0     2024 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payments_related_documents_sat.py
+-rw-r--r--   0        0        0     3037 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payments_sat.py
+-rw-r--r--   0        0        0     2066 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payroll_dian.py
+-rw-r--r--   0        0        0     1782 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_payroll_sat.py
+-rw-r--r--   0        0        0     2343 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_receiver_details_dian.py
+-rw-r--r--   0        0        0     2061 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_request.py
+-rw-r--r--   0        0        0     1809 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_response_paginated_response.py
+-rw-r--r--   0        0        0      260 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/invoices_response_paginated_response_results_item.py
+-rw-r--r--   0        0        0     1249 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_invalid_credentials.py
+-rw-r--r--   0        0        0     1227 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_invalid_token.py
+-rw-r--r--   0        0        0     1257 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_login_error.py
+-rw-r--r--   0        0        0     1243 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_payment_error.py
+-rw-r--r--   0        0        0     1289 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_session_expired.py
+-rw-r--r--   0        0        0     1261 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/last_error_two_factor.py
+-rw-r--r--   0        0        0     2833 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/link.py
+-rw-r--r--   0        0        0     4669 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/links_put_request.py
+-rw-r--r--   0        0        0     7955 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/links_request.py
+-rw-r--r--   0        0        0      554 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/list_payment_links_request_ordering.py
+-rw-r--r--   0        0        0      521 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/list_payment_links_request_status.py
+-rw-r--r--   0        0        0      356 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/list_tax_declarations_response.py
+-rw-r--r--   0        0        0      586 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/list_tax_returns_response.py
+-rw-r--r--   0        0        0     2699 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/login_error.py
+-rw-r--r--   0        0        0      913 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/needs_redirect_content.py
+-rw-r--r--   0        0        0      923 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/needs_redirect_content_pse.py
+-rw-r--r--   0        0        0     1588 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/net_income_individual.py
+-rw-r--r--   0        0        0     1660 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_ofpi.py
+-rw-r--r--   0        0        0     2256 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py
+-rw-r--r--   0        0        0     1673 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_pse.py
+-rw-r--r--   0        0        0     2850 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_pse_type.py
+-rw-r--r--   0        0        0     1665 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_credentials_required_pse.py
+-rw-r--r--   0        0        0     2840 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_credentials_required_pse_type.py
+-rw-r--r--   0        0        0     1676 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_customer_bank_accounts_pse.py
+-rw-r--r--   0        0        0     2850 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py
+-rw-r--r--   0        0        0     1595 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_needs_redirect_pse.py
+-rw-r--r--   0        0        0     2780 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_needs_redirect_pse_type.py
+-rw-r--r--   0        0        0     1573 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_failed.py
+-rw-r--r--   0        0        0     2179 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_failed_type.py
+-rw-r--r--   0        0        0     1700 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information.py
+-rw-r--r--   0        0        0     1874 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_pse.py
+-rw-r--r--   0        0        0     2890 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_pse_type.py
+-rw-r--r--   0        0        0     2256 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_type.py
+-rw-r--r--   0        0        0     1606 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_processing.py
+-rw-r--r--   0        0        0     2207 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_processing_type.py
+-rw-r--r--   0        0        0     1598 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_succeeded.py
+-rw-r--r--   0        0        0     2200 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_succeeded_type.py
+-rw-r--r--   0        0        0     2128 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_token_required_pse.py
+-rw-r--r--   0        0        0     2780 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_display_token_required_pse_type.py
+-rw-r--r--   0        0        0     1545 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_needs_redirect.py
+-rw-r--r--   0        0        0     2130 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/next_step_needs_redirect_type.py
+-rw-r--r--   0        0        0     1531 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/non_taxable_income_individual.py
+-rw-r--r--   0        0        0     1703 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/not_found_error_body.py
+-rw-r--r--   0        0        0     2545 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/owner.py
+-rw-r--r--   0        0        0     1584 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/owner_document_id.py
+-rw-r--r--   0        0        0     1661 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/owners_paginated_response.py
+-rw-r--r--   0        0        0     1596 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/paginated_response_link.py
+-rw-r--r--   0        0        0     1798 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/patch_body.py
+-rw-r--r--   0        0        0     1479 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/patch_body_without_save_data.py
+-rw-r--r--   0        0        0      241 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/patch_invoices_response_item.py
+-rw-r--r--   0        0        0      876 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/patch_payment_intents_body_pse.py
+-rw-r--r--   0        0        0     2677 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/patch_payment_method_details_pse.py
+-rw-r--r--   0        0        0     2302 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_institution.py
+-rw-r--r--   0        0        0     4025 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_ofpi.py
+-rw-r--r--   0        0        0      846 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_ofpi_next_step.py
+-rw-r--r--   0        0        0      462 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_ofpi_payment_method_details.py
+-rw-r--r--   0        0        0     1733 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_paginated_response.py
+-rw-r--r--   0        0        0     1549 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py
+-rw-r--r--   0        0        0     1551 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py
+-rw-r--r--   0        0        0     2222 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0     1013 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py
+-rw-r--r--   0        0        0     1030 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py
+-rw-r--r--   0        0        0      983 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_pse.py
+-rw-r--r--   0        0        0     4050 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_pse.py
+-rw-r--r--   0        0        0      656 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_pse_last_error.py
+-rw-r--r--   0        0        0      933 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intent_pse_next_step.py
+-rw-r--r--   0        0        0     1644 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intents_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0      995 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_intents_payment_method_details_pse.py
+-rw-r--r--   0        0        0     1499 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_callback_urls.py
+-rw-r--r--   0        0        0     1408 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_callback_urls_response.py
+-rw-r--r--   0        0        0     2547 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_list_ofpi.py
+-rw-r--r--   0        0        0     2546 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_list_pse.py
+-rw-r--r--   0        0        0     2331 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_ofpi.py
+-rw-r--r--   0        0        0     1801 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_paginated_response.py
+-rw-r--r--   0        0        0      287 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_paginated_response_results_item.py
+-rw-r--r--   0        0        0     2326 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_link_pse.py
+-rw-r--r--   0        0        0     1244 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_links_payment_method_details_body_ofpi.py
+-rw-r--r--   0        0        0     1646 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_links_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0     1021 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_details_ofpi.py
+-rw-r--r--   0        0        0      980 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_details_pse.py
+-rw-r--r--   0        0        0     1530 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py
+-rw-r--r--   0        0        0     1256 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_information_body_ofpi.py
+-rw-r--r--   0        0        0     1390 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_information_body_pse.py
+-rw-r--r--   0        0        0     1013 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_information_details_pse.py
+-rw-r--r--   0        0        0      967 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_information_ofpi.py
+-rw-r--r--   0        0        0     1043 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_method_information_pse.py
+-rw-r--r--   0        0        0     2247 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_transaction.py
+-rw-r--r--   0        0        0      313 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_transaction_payer.py
+-rw-r--r--   0        0        0     1527 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payment_webhook.py
+-rw-r--r--   0        0        0     1742 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payments_institutions_paginated_response.py
+-rw-r--r--   0        0        0     1742 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payments_transactions_paginated_response.py
+-rw-r--r--   0        0        0     1471 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payments_way.py
+-rw-r--r--   0        0        0     1708 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/payments_webhooks_paginated_response.py
+-rw-r--r--   0        0        0     1072 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/pension_income_statement_individual.py
+-rw-r--r--   0        0        0      817 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/providers_pse.py
+-rw-r--r--   0        0        0     1866 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/receivable_transaction_request.py
+-rw-r--r--   0        0        0     2957 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/receivables_transaction.py
+-rw-r--r--   0        0        0     1042 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/receivables_transaction_account.py
+-rw-r--r--   0        0        0     1065 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/receivables_transaction_number_of_installments.py
+-rw-r--r--   0        0        0     1750 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/receivables_transactions_paginated_response.py
+-rw-r--r--   0        0        0     1026 2023-05-12 20:16:51.715496 fern_belvo-0.0.24/src/belvo/types/recevables_transaction_fees.py
+-rw-r--r--   0        0        0     1242 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/recurring_expense_source_transaction.py
+-rw-r--r--   0        0        0     2895 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/recurring_expenses.py
+-rw-r--r--   0        0        0     1735 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/recurring_expenses_paginated_response.py
+-rw-r--r--   0        0        0     2148 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/recurring_expenses_request.py
+-rw-r--r--   0        0        0     1120 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/reporting_id.py
+-rw-r--r--   0        0        0     2051 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/request_timeout_error_body.py
+-rw-r--r--   0        0        0     1454 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retention_breakdown.py
+-rw-r--r--   0        0        0      244 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retrieve_invoices_response_item.py
+-rw-r--r--   0        0        0      308 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retrieve_tax_declarations_response_item.py
+-rw-r--r--   0        0        0      307 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retrieve_tax_returns_request_body.py
+-rw-r--r--   0        0        0      457 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retrieve_tax_returns_response_item.py
+-rw-r--r--   0        0        0      235 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/retrieve_tax_status_response.py
+-rw-r--r--   0        0        0     1980 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights.py
+-rw-r--r--   0        0        0     3951 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_balance_metrics.py
+-rw-r--r--   0        0        0     3942 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_cashflow_metrics.py
+-rw-r--r--   0        0        0     1093 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_credit_card_metrics.py
+-rw-r--r--   0        0        0     1369 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_loans_metrics.py
+-rw-r--r--   0        0        0     1711 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_paginated_response.py
+-rw-r--r--   0        0        0     9169 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/risk_insights_transaction_metrics.py
+-rw-r--r--   0        0        0     1176 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/secret_keys.py
+-rw-r--r--   0        0        0     1694 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/secret_keys_paginated_response.py
+-rw-r--r--   0        0        0     2013 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/session_expired_error.py
+-rw-r--r--   0        0        0     1276 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/standard_request.py
+-rw-r--r--   0        0        0     2491 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_assessment_business.py
+-rw-r--r--   0        0        0     2771 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_assessment_individual.py
+-rw-r--r--   0        0        0     1788 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_compliance_status.py
+-rw-r--r--   0        0        0     1748 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_compliance_status_paginated_response.py
+-rw-r--r--   0        0        0     1326 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_compliance_status_request.py
+-rw-r--r--   0        0        0     2291 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_declaration_business.py
+-rw-r--r--   0        0        0     1755 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_declaration_business_paginated.py
+-rw-r--r--   0        0        0     2281 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_declaration_individual.py
+-rw-r--r--   0        0        0     1765 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_declaration_individual_paginated.py
+-rw-r--r--   0        0        0     1727 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_declarations_request.py
+-rw-r--r--   0        0        0     1666 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_payer_information_business.py
+-rw-r--r--   0        0        0     1489 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_payer_information_individual.py
+-rw-r--r--   0        0        0     3880 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_retentions.py
+-rw-r--r--   0        0        0     1716 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_retentions_paginated_response.py
+-rw-r--r--   0        0        0     1989 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_retentions_request.py
+-rw-r--r--   0        0        0      129 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_return_business.py
+-rw-r--r--   0        0        0      136 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_return_business_monthly.py
+-rw-r--r--   0        0        0      129 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_return_personal.py
+-rw-r--r--   0        0        0      136 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_return_personal_monthly.py
+-rw-r--r--   0        0        0      146 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_business_monthly_paginated.py
+-rw-r--r--   0        0        0      139 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_business_paginated.py
+-rw-r--r--   0        0        0     2175 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_monthly_request.py
+-rw-r--r--   0        0        0      146 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_personal_monthly_paginated.py
+-rw-r--r--   0        0        0      139 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_personal_paginated.py
+-rw-r--r--   0        0        0     1967 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_returns_yearly_request.py
+-rw-r--r--   0        0        0     1089 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_address_between_street_dian.py
+-rw-r--r--   0        0        0     1029 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_address_between_street_sat.py
+-rw-r--r--   0        0        0     2076 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_address_dian.py
+-rw-r--r--   0        0        0     1919 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_address_sat.py
+-rw-r--r--   0        0        0     3269 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_dian.py
+-rw-r--r--   0        0        0     1728 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_economic_activity_dian.py
+-rw-r--r--   0        0        0     1328 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_economic_activity_sat.py
+-rw-r--r--   0        0        0     1550 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_obligations_dian.py
+-rw-r--r--   0        0        0     1357 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_obligations_sat.py
+-rw-r--r--   0        0        0     1784 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_paginated_response.py
+-rw-r--r--   0        0        0      247 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_paginated_response_results_item.py
+-rw-r--r--   0        0        0     1179 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_regimens_dian.py
+-rw-r--r--   0        0        0     1048 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_regimens_sat.py
+-rw-r--r--   0        0        0     1316 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_request.py
+-rw-r--r--   0        0        0     3194 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_sat.py
+-rw-r--r--   0        0        0     2648 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_tax_payer_information_dian.py
+-rw-r--r--   0        0        0     2672 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/tax_status_tax_payer_information_sat.py
+-rw-r--r--   0        0        0     2428 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/token_required_response.py
+-rw-r--r--   0        0        0     1605 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/token_required_response_token_generation_data.py
+-rw-r--r--   0        0        0     2133 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/too_many_sessions_error.py
+-rw-r--r--   0        0        0     3391 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction.py
+-rw-r--r--   0        0        0     1052 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction_bank_account_body_pse.py
+-rw-r--r--   0        0        0      138 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction_bank_account_ofpi.py
+-rw-r--r--   0        0        0      325 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction_bank_account_pse.py
+-rw-r--r--   0        0        0     1689 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction_credit_card_data.py
+-rw-r--r--   0        0        0     1049 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transaction_merchant_data.py
+-rw-r--r--   0        0        0     1691 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transactions_paginated_response.py
+-rw-r--r--   0        0        0     2001 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/transactions_request.py
+-rw-r--r--   0        0        0     1945 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     2077 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/unconfirmed_link_error.py
+-rw-r--r--   0        0        0     2013 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/unexpected_error.py
+-rw-r--r--   0        0        0     2032 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/unsupported_operation_error.py
+-rw-r--r--   0        0        0     2657 2023-05-12 20:16:51.719496 fern_belvo-0.0.24/src/belvo/types/validation_error.py
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 fern_belvo-0.0.24/PKG-INFO
```

### Comparing `fern_belvo-0.0.23/README.md` & `fern_belvo-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/__init__.py` & `fern_belvo-0.0.24/src/belvo/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/core/datetime_utils.py` & `fern_belvo-0.0.24/src/belvo/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/core/jsonable_encoder.py` & `fern_belvo-0.0.24/src/belvo/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/errors/__init__.py` & `fern_belvo-0.0.24/src/belvo/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/resources/__init__.py` & `fern_belvo-0.0.24/src/belvo/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/resources/accounts/client.py` & `fern_belvo-0.0.24/src/belvo/resources/accounts/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from ...types.standard_request import StandardRequest
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class AccountsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_accounts(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -115,16 +117,16 @@
                 "name__icontains": name_icontains,
                 "number": number,
                 "number__in": number_in,
                 "public_identification_name": public_identification_name,
                 "public_identification_value": public_identification_value,
                 "type": type,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -140,16 +142,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
     ) -> typing.List[Account]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -181,16 +183,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
     ) -> typing.List[Account]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -221,16 +223,16 @@
     def detail_account(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Account:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -244,16 +246,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_account(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -265,18 +267,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAccountsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_accounts(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -356,16 +360,16 @@
                     "name__icontains": name_icontains,
                     "number": number,
                     "number__in": number_in,
                     "public_identification_name": public_identification_name,
                     "public_identification_value": public_identification_value,
                     "type": type,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -382,16 +386,16 @@
     ) -> typing.List[Account]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -424,16 +428,16 @@
     ) -> typing.List[Account]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -465,16 +469,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Account:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -489,16 +493,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_account(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/balances/client.py` & `fern_belvo-0.0.24/src/belvo/resources/balances/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class BalancesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_balances(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -95,16 +97,16 @@
                 "value_date": value_date,
                 "value_date__gt": value_date_gt,
                 "value_date__gte": value_date_gte,
                 "value_date__lt": value_date_lt,
                 "value_date__lte": value_date_lte,
                 "value_date__range": value_date_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BalancesPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -120,16 +122,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: BalancesRequest
     ) -> typing.List[Balance]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/balances"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Balance], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -161,16 +163,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
     ) -> typing.List[Balance]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/balances"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Balance], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -201,16 +203,16 @@
     def detail_balance(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Balance:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/balances/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Balance, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -224,16 +226,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_balance(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/balances/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -245,18 +247,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncBalancesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_balances(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -316,16 +320,16 @@
                     "value_date": value_date,
                     "value_date__gt": value_date_gt,
                     "value_date__gte": value_date_gte,
                     "value_date__lt": value_date_lt,
                     "value_date__lte": value_date_lte,
                     "value_date__range": value_date_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BalancesPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -342,16 +346,16 @@
     ) -> typing.List[Balance]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/balances"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Balance], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -384,16 +388,16 @@
     ) -> typing.List[Balance]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/balances"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Balance], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -425,16 +429,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Balance:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/balances/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Balance, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -449,16 +453,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_balance(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/balances/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/bank_accounts/client.py` & `fern_belvo-0.0.24/src/belvo/resources/customers/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,257 +9,231 @@
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
-from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.bank_account_paginated_response import BankAccountPaginatedResponse
-from ...types.create_bank_account_request import CreateBankAccountRequest
-from ...types.create_bank_account_response import CreateBankAccountResponse
-from ...types.detail_bank_account_response import DetailBankAccountResponse
+from ...types.create_customer_request import CreateCustomerRequest
+from ...types.create_customer_response import CreateCustomerResponse
+from ...types.customer_paginated_response import CustomerPaginatedResponse
+from ...types.detail_customer_response import DetailCustomerResponse
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class BankAccountsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class CustomersClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_bank_account(
+    def list_customers(
         self,
         *,
         page: typing.Optional[int] = None,
         id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        number: typing.Optional[str] = None,
-        number_in: typing.Optional[str] = None,
-        customer: typing.Optional[str] = None,
-        institution: typing.Optional[str] = None,
-        holder_type: typing.Optional[str] = None,
-        holder_type_in: typing.Optional[str] = None,
-        providers: typing.Optional[str] = None,
-    ) -> BankAccountPaginatedResponse:
+        customer_type: typing.Optional[str] = None,
+        search: typing.Optional[str] = None,
+    ) -> CustomerPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
             params={
                 "page": page,
                 "id__in": id_in,
                 "created_at": created_at,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
-                "number": number,
-                "number__in": number_in,
-                "customer": customer,
-                "institution": institution,
-                "holder__type": holder_type,
-                "holder__type__in": holder_type_in,
-                "providers": providers,
+                "customer__type": customer_type,
+                "search": search,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BankAccountPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CustomerPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_bank_account(self, *, request: CreateBankAccountRequest) -> CreateBankAccountResponse:
+    def create_customer(self, *, request: CreateCustomerRequest) -> CreateCustomerResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateBankAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateCustomerResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 408:
-            raise RequestTimeoutError(
-                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_bank_account(self, id: str) -> DetailBankAccountResponse:
+    def detail_customer(self, id: str) -> DetailCustomerResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/bank-accounts/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/customers/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailBankAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailCustomerResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncBankAccountsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncCustomersClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_bank_account(
+    async def list_customers(
         self,
         *,
         page: typing.Optional[int] = None,
         id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        number: typing.Optional[str] = None,
-        number_in: typing.Optional[str] = None,
-        customer: typing.Optional[str] = None,
-        institution: typing.Optional[str] = None,
-        holder_type: typing.Optional[str] = None,
-        holder_type_in: typing.Optional[str] = None,
-        providers: typing.Optional[str] = None,
-    ) -> BankAccountPaginatedResponse:
+        customer_type: typing.Optional[str] = None,
+        search: typing.Optional[str] = None,
+    ) -> CustomerPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
                 params={
                     "page": page,
                     "id__in": id_in,
                     "created_at": created_at,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
-                    "number": number,
-                    "number__in": number_in,
-                    "customer": customer,
-                    "institution": institution,
-                    "holder__type": holder_type,
-                    "holder__type__in": holder_type_in,
-                    "providers": providers,
+                    "customer__type": customer_type,
+                    "search": search,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BankAccountPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CustomerPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_bank_account(self, *, request: CreateBankAccountRequest) -> CreateBankAccountResponse:
+    async def create_customer(self, *, request: CreateCustomerRequest) -> CreateCustomerResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateBankAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateCustomerResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 408:
-            raise RequestTimeoutError(
-                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_bank_account(self, id: str) -> DetailBankAccountResponse:
+    async def detail_customer(self, id: str) -> DetailCustomerResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/bank-accounts/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/customers/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailBankAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailCustomerResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/customers/client.py` & `fern_belvo-0.0.24/src/belvo/resources/payment_links/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,227 +9,247 @@
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
+from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.create_customer_request import CreateCustomerRequest
-from ...types.create_customer_response import CreateCustomerResponse
-from ...types.customer_paginated_response import CustomerPaginatedResponse
-from ...types.detail_customer_response import DetailCustomerResponse
+from ...types.create_paymentlink_request import CreatePaymentlinkRequest
+from ...types.create_paymentlink_response import CreatePaymentlinkResponse
+from ...types.detail_create_paymentlink_response import DetailCreatePaymentlinkResponse
+from ...types.list_payment_links_request_ordering import ListPaymentLinksRequestOrdering
+from ...types.list_payment_links_request_status import ListPaymentLinksRequestStatus
 from ...types.not_found_error_body import NotFoundErrorBody
+from ...types.payment_link_paginated_response import PaymentLinkPaginatedResponse
+from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class CustomersClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class PaymentLinksClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_customers(
+    def list_payment_links(
         self,
         *,
         page: typing.Optional[int] = None,
-        id_in: typing.Optional[str] = None,
+        page_size: typing.Optional[int] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        customer_type: typing.Optional[str] = None,
+        status: typing.Optional[ListPaymentLinksRequestStatus] = None,
+        ordering: typing.Optional[ListPaymentLinksRequestOrdering] = None,
         search: typing.Optional[str] = None,
-    ) -> CustomerPaginatedResponse:
+    ) -> PaymentLinkPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
             params={
                 "page": page,
-                "id__in": id_in,
+                "page_size": page_size,
                 "created_at": created_at,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
-                "customer__type": customer_type,
+                "status": status,
+                "ordering": ordering,
                 "search": search,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CustomerPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentLinkPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_customer(self, *, request: CreateCustomerRequest) -> CreateCustomerResponse:
+    def create_paymentlink(self, *, request: CreatePaymentlinkRequest) -> CreatePaymentlinkResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateCustomerResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreatePaymentlinkResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
+        if _response.status_code == 408:
+            raise RequestTimeoutError(
+                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
+            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_customer(self, id: str) -> DetailCustomerResponse:
+    def detail_create_paymentlink(self, access_token: str) -> DetailCreatePaymentlinkResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/customers/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-links/{access_token}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailCustomerResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailCreatePaymentlinkResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncCustomersClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncPaymentLinksClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_customers(
+    async def list_payment_links(
         self,
         *,
         page: typing.Optional[int] = None,
-        id_in: typing.Optional[str] = None,
+        page_size: typing.Optional[int] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        customer_type: typing.Optional[str] = None,
+        status: typing.Optional[ListPaymentLinksRequestStatus] = None,
+        ordering: typing.Optional[ListPaymentLinksRequestOrdering] = None,
         search: typing.Optional[str] = None,
-    ) -> CustomerPaginatedResponse:
+    ) -> PaymentLinkPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
                 params={
                     "page": page,
-                    "id__in": id_in,
+                    "page_size": page_size,
                     "created_at": created_at,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
-                    "customer__type": customer_type,
+                    "status": status,
+                    "ordering": ordering,
                     "search": search,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CustomerPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentLinkPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_customer(self, *, request: CreateCustomerRequest) -> CreateCustomerResponse:
+    async def create_paymentlink(self, *, request: CreatePaymentlinkRequest) -> CreatePaymentlinkResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/customers"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateCustomerResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreatePaymentlinkResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
+        if _response.status_code == 408:
+            raise RequestTimeoutError(
+                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
+            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_customer(self, id: str) -> DetailCustomerResponse:
+    async def detail_create_paymentlink(self, access_token: str) -> DetailCreatePaymentlinkResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/customers/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-links/{access_token}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailCustomerResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailCreatePaymentlinkResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/employment_records/client.py` & `fern_belvo-0.0.24/src/belvo/resources/tax_compliance_status/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,140 +9,159 @@
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
-from ...errors.precondition_error import PreconditionError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.employment_record import EmploymentRecord
-from ...types.employment_record_request import EmploymentRecordRequest
-from ...types.employment_records_paginated_response import EmploymentRecordsPaginatedResponse
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
-from ...types.token_required_response import TokenRequiredResponse
+from ...types.tax_compliance_status import TaxComplianceStatus
+from ...types.tax_compliance_status_paginated_response import TaxComplianceStatusPaginatedResponse
+from ...types.tax_compliance_status_request import TaxComplianceStatusRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class EmploymentRecordsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class TaxComplianceStatusClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_employment_records(
+    def list_tax_compliance_status(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-    ) -> EmploymentRecordsPaginatedResponse:
+        link: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+    ) -> TaxComplianceStatusPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
-            params={"page": page, "page_size": page_size, "omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+            params={
+                "page": page,
+                "page_size": page_size,
+                "omit": omit,
+                "fields": fields,
+                "link": link,
+                "created_at__gt": created_at_gt,
+                "created_at__gte": created_at_gte,
+                "created_at__lt": created_at_lt,
+                "created_at__lte": created_at_lte,
+                "created_at__range": created_at_range,
+                "id": id,
+                "id__in": id_in,
+                "link__in": link_in,
+            },
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EmploymentRecordsPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatusPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_employment_record_details(
+    def retrieve_tax_compliance_status(
         self,
         *,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        request: EmploymentRecordRequest,
-    ) -> typing.List[EmploymentRecord]:
+        request: TaxComplianceStatusRequest,
+    ) -> TaxComplianceStatus:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EmploymentRecord], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_employment_record(
+    def detail_tax_compliance_status(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> EmploymentRecord:
+    ) -> TaxComplianceStatus:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EmploymentRecord, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_employment_record(self, id: str) -> None:
+    def destroy_tax_compliance_status(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -153,130 +172,151 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncEmploymentRecordsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncTaxComplianceStatusClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_employment_records(
+    async def list_tax_compliance_status(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-    ) -> EmploymentRecordsPaginatedResponse:
+        link: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+    ) -> TaxComplianceStatusPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
-                params={"page": page, "page_size": page_size, "omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+                params={
+                    "page": page,
+                    "page_size": page_size,
+                    "omit": omit,
+                    "fields": fields,
+                    "link": link,
+                    "created_at__gt": created_at_gt,
+                    "created_at__gte": created_at_gte,
+                    "created_at__lt": created_at_lt,
+                    "created_at__lte": created_at_lte,
+                    "created_at__range": created_at_range,
+                    "id": id,
+                    "id__in": id_in,
+                    "link__in": link_in,
+                },
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EmploymentRecordsPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatusPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_employment_record_details(
+    async def retrieve_tax_compliance_status(
         self,
         *,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        request: EmploymentRecordRequest,
-    ) -> typing.List[EmploymentRecord]:
+        request: TaxComplianceStatusRequest,
+    ) -> TaxComplianceStatus:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EmploymentRecord], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_employment_record(
+    async def detail_tax_compliance_status(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> EmploymentRecord:
+    ) -> TaxComplianceStatus:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EmploymentRecord, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_employment_record(self, id: str) -> None:
+    async def destroy_tax_compliance_status(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/income_verification/client.py` & `fern_belvo-0.0.24/src/belvo/resources/income_verification/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 from ...types.unexpected_error import UnexpectedError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class IncomeVerificationClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def verify_income(
         self,
         *,
         language: str,
         transactions: typing.List[EyodIncomeVerificationBodyRequest],
         date_from: typing.Optional[str] = OMIT,
@@ -52,16 +54,16 @@
             _request["allowed_income_types"] = allowed_income_types
         if minimum_confidence_level is not OMIT:
             _request["minimum_confidence_level"] = minimum_confidence_level
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/enrich/incomes"),
             json=jsonable_encoder(_request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -83,18 +85,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncIncomeVerificationClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def verify_income(
         self,
         *,
         language: str,
         transactions: typing.List[EyodIncomeVerificationBodyRequest],
         date_from: typing.Optional[str] = OMIT,
@@ -112,16 +116,16 @@
         if minimum_confidence_level is not OMIT:
             _request["minimum_confidence_level"] = minimum_confidence_level
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/enrich/incomes"),
                 json=jsonable_encoder(_request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/incomes/client.py` & `fern_belvo-0.0.24/src/belvo/resources/owners/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,88 +13,104 @@
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.precondition_error import PreconditionError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.income import Income
-from ...types.incomes_paginated_response import IncomesPaginatedResponse
-from ...types.incomes_request import IncomesRequest
 from ...types.not_found_error_body import NotFoundErrorBody
+from ...types.owner import Owner
+from ...types.owners_paginated_response import OwnersPaginatedResponse
 from ...types.patch_body import PatchBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
+from ...types.standard_request import StandardRequest
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class IncomesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class OwnersClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_incomes(
+    def list_owners(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        account: typing.Optional[str] = None,
-        account_in: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
+        display_name_icontains: typing.Optional[str] = None,
+        email: typing.Optional[str] = None,
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> IncomesPaginatedResponse:
+    ) -> OwnersPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
             params={
                 "page": page,
                 "page_size": page_size,
                 "omit": omit,
                 "fields": fields,
-                "account": account,
-                "account__in": account_in,
+                "created_at__gt": created_at_gt,
+                "created_at__gte": created_at_gte,
+                "created_at__lt": created_at_lt,
+                "created_at__lte": created_at_lte,
+                "created_at__range": created_at_range,
+                "display_name__icontains": display_name_icontains,
+                "email": email,
+                "id": id,
+                "id__in": id_in,
                 "link": link,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(IncomesPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OwnersPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_income(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: IncomesRequest
-    ) -> Income:
+    def retrieve_owners(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
+    ) -> typing.List[Owner]:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Income, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -113,29 +129,29 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def patch_incomes(
+    def patch_owners(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Income]:
+    ) -> typing.List[Owner]:
         _response = httpx.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -154,46 +170,44 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_income(
-        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> typing.List[Income]:
+    def detail_owner(self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None) -> Owner:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/incomes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Owner, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_incomes(self, id: str) -> None:
+    def destroy_owner(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/incomes/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -204,79 +218,95 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncIncomesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncOwnersClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_incomes(
+    async def list_owners(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        account: typing.Optional[str] = None,
-        account_in: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
+        display_name_icontains: typing.Optional[str] = None,
+        email: typing.Optional[str] = None,
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> IncomesPaginatedResponse:
+    ) -> OwnersPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
                 params={
                     "page": page,
                     "page_size": page_size,
                     "omit": omit,
                     "fields": fields,
-                    "account": account,
-                    "account__in": account_in,
+                    "created_at__gt": created_at_gt,
+                    "created_at__gte": created_at_gte,
+                    "created_at__lt": created_at_lt,
+                    "created_at__lte": created_at_lte,
+                    "created_at__range": created_at_range,
+                    "display_name__icontains": display_name_icontains,
+                    "email": email,
+                    "id": id,
+                    "id__in": id_in,
                     "link": link,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(IncomesPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OwnersPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_income(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: IncomesRequest
-    ) -> Income:
+    async def retrieve_owners(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
+    ) -> typing.List[Owner]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Income, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -295,30 +325,30 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def patch_incomes(
+    async def patch_owners(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Income]:
+    ) -> typing.List[Owner]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/incomes"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -337,48 +367,48 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_income(
+    async def detail_owner(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> typing.List[Income]:
+    ) -> Owner:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/incomes/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Income], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Owner, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_incomes(self, id: str) -> None:
+    async def destroy_owner(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/incomes/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/institutions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/institutions/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ...types.institution import Institution
 from ...types.institutions_paginated_response import InstitutionsPaginatedResponse
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 
 
 class InstitutionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_institutions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -58,16 +60,16 @@
                 "resources__allin": resources_allin,
                 "status": status,
                 "status__in": status_in,
                 "type": type,
                 "type__in": type_in,
                 "website": website,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InstitutionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -82,16 +84,16 @@
     def detail_institution(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Institution:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/institutions/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Institution, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -103,18 +105,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncInstitutionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_institutions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -148,16 +152,16 @@
                     "resources__allin": resources_allin,
                     "status": status,
                     "status__in": status_in,
                     "type": type,
                     "type__in": type_in,
                     "website": website,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InstitutionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -173,16 +177,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Institution:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/institutions/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Institution, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/investment_portfolios/client.py` & `fern_belvo-0.0.24/src/belvo/resources/investment_portfolios/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 from ...types.standard_request import StandardRequest
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class InvestmentPortfoliosClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_portfolio(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -59,16 +61,16 @@
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfoliosPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -84,16 +86,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
     ) -> InvestmentsPortfolio:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "investments/portfolios"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -125,16 +127,16 @@
         request: PatchBodyWithoutSaveData,
     ) -> InvestmentsPortfolio:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "investments/portfolios"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -161,16 +163,16 @@
     def detail_portfolio(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> InvestmentsPortfolio:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"investments/portfolios/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -184,16 +186,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_portfolio(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"investments/portfolios/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -205,18 +207,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncInvestmentPortfoliosClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_portfolio(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -242,16 +246,16 @@
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfoliosPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -268,16 +272,16 @@
     ) -> InvestmentsPortfolio:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "investments/portfolios"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -310,16 +314,16 @@
     ) -> InvestmentsPortfolio:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "investments/portfolios"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -347,16 +351,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> InvestmentsPortfolio:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"investments/portfolios/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvestmentsPortfolio, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -371,16 +375,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_portfolio(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"investments/portfolios/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/invoices/client.py` & `fern_belvo-0.0.24/src/belvo/resources/invoices/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 from ...types.retrieve_invoices_response_item import RetrieveInvoicesResponseItem
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class InvoicesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_invoices(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -103,16 +105,16 @@
                 "total_amount__lte": total_amount_lte,
                 "total_amount__gt": total_amount_gt,
                 "total_amount__gte": total_amount_gte,
                 "total_amount__range": total_amount_range,
                 "type": type,
                 "type__in": type_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoicesResponsePaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -128,16 +130,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: InvoicesRequest
     ) -> typing.List[RetrieveInvoicesResponseItem]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/invoices"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RetrieveInvoicesResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -165,16 +167,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
     ) -> typing.List[PatchInvoicesResponseItem]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/invoices"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PatchInvoicesResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -205,16 +207,16 @@
     def detail_invoice(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> DetailInvoiceResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/invoices/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailInvoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -228,16 +230,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_invoice(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/invoices/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -249,18 +251,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncInvoicesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_invoices(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -326,16 +330,16 @@
                     "total_amount__lte": total_amount_lte,
                     "total_amount__gt": total_amount_gt,
                     "total_amount__gte": total_amount_gte,
                     "total_amount__range": total_amount_range,
                     "type": type,
                     "type__in": type_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoicesResponsePaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -352,16 +356,16 @@
     ) -> typing.List[RetrieveInvoicesResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/invoices"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RetrieveInvoicesResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -390,16 +394,16 @@
     ) -> typing.List[PatchInvoicesResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/invoices"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PatchInvoicesResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -431,16 +435,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> DetailInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/invoices/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailInvoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -455,16 +459,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_invoice(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/invoices/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/links/client.py` & `fern_belvo-0.0.24/src/belvo/resources/links/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from ...types.patch_body_without_save_data import PatchBodyWithoutSaveData
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class LinksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_links(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -85,16 +87,16 @@
                 "institution__in": institution_in,
                 "institution_user_id": institution_user_id,
                 "institution_user_id__in": institution_user_id_in,
                 "refresh_rate": refresh_rate,
                 "status": status,
                 "status__in": status_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResponseLink, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -110,16 +112,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: LinksRequest
     ) -> Link:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/links"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -151,16 +153,16 @@
         request: PatchBodyWithoutSaveData,
     ) -> Link:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/links"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -185,16 +187,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detail_link(self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None) -> Link:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -217,16 +219,16 @@
         request: LinksPutRequest,
     ) -> Link:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -261,16 +263,16 @@
         request: ChangeAccessMode,
     ) -> Link:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -296,16 +298,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_link(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -317,18 +319,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncLinksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_links(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -378,16 +382,16 @@
                     "institution__in": institution_in,
                     "institution_user_id": institution_user_id,
                     "institution_user_id__in": institution_user_id_in,
                     "refresh_rate": refresh_rate,
                     "status": status,
                     "status__in": status_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResponseLink, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -404,16 +408,16 @@
     ) -> Link:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/links"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -446,16 +450,16 @@
     ) -> Link:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/links"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -483,16 +487,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Link:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -516,16 +520,16 @@
     ) -> Link:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -561,16 +565,16 @@
     ) -> Link:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Link, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -597,16 +601,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_link(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/links/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/owners/client.py` & `fern_belvo-0.0.24/src/belvo/resources/risk_insights/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,101 +14,89 @@
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.precondition_error import PreconditionError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.owner import Owner
-from ...types.owners_paginated_response import OwnersPaginatedResponse
 from ...types.patch_body import PatchBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
+from ...types.risk_insights import RiskInsights
+from ...types.risk_insights_paginated_response import RiskInsightsPaginatedResponse
 from ...types.standard_request import StandardRequest
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class OwnersClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class RiskInsightsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_owners(
+    def list_risk_insights(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        created_at_gt: typing.Optional[str] = None,
-        created_at_gte: typing.Optional[str] = None,
-        created_at_lt: typing.Optional[str] = None,
-        created_at_lte: typing.Optional[str] = None,
-        created_at_range: typing.Optional[str] = None,
-        display_name_icontains: typing.Optional[str] = None,
-        email: typing.Optional[str] = None,
+        link: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> OwnersPaginatedResponse:
+    ) -> RiskInsightsPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
             params={
                 "page": page,
                 "page_size": page_size,
                 "omit": omit,
                 "fields": fields,
-                "created_at__gt": created_at_gt,
-                "created_at__gte": created_at_gte,
-                "created_at__lt": created_at_lt,
-                "created_at__lte": created_at_lte,
-                "created_at__range": created_at_range,
-                "display_name__icontains": display_name_icontains,
-                "email": email,
+                "link": link,
                 "id": id,
                 "id__in": id_in,
-                "link": link,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OwnersPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RiskInsightsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_owners(
+    def retrieve_risk_insights(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[Owner]:
+    ) -> typing.List[RiskInsights]:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -127,29 +115,29 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def patch_owners(
+    def patch_risk_insights(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Owner]:
+    ) -> typing.List[RiskInsights]:
         _response = httpx.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -168,44 +156,46 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_owner(self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None) -> Owner:
+    def detail_risk_insights(
+        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
+    ) -> typing.List[RiskInsights]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Owner, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_owner(self, id: str) -> None:
+    def destroy_risk_insights(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -216,93 +206,81 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncOwnersClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncRiskInsightsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_owners(
+    async def list_risk_insights(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        created_at_gt: typing.Optional[str] = None,
-        created_at_gte: typing.Optional[str] = None,
-        created_at_lt: typing.Optional[str] = None,
-        created_at_lte: typing.Optional[str] = None,
-        created_at_range: typing.Optional[str] = None,
-        display_name_icontains: typing.Optional[str] = None,
-        email: typing.Optional[str] = None,
+        link: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> OwnersPaginatedResponse:
+    ) -> RiskInsightsPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
                 params={
                     "page": page,
                     "page_size": page_size,
                     "omit": omit,
                     "fields": fields,
-                    "created_at__gt": created_at_gt,
-                    "created_at__gte": created_at_gte,
-                    "created_at__lt": created_at_lt,
-                    "created_at__lte": created_at_lte,
-                    "created_at__range": created_at_range,
-                    "display_name__icontains": display_name_icontains,
-                    "email": email,
+                    "link": link,
                     "id": id,
                     "id__in": id_in,
-                    "link": link,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OwnersPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RiskInsightsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_owners(
+    async def retrieve_risk_insights(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[Owner]:
+    ) -> typing.List[RiskInsights]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -321,30 +299,30 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def patch_owners(
+    async def patch_risk_insights(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Owner]:
+    ) -> typing.List[RiskInsights]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/owners"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Owner], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -363,48 +341,48 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_owner(
+    async def detail_risk_insights(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> Owner:
+    ) -> typing.List[RiskInsights]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Owner, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_owner(self, id: str) -> None:
+    async def destroy_risk_insights(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/owners/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/payment_institutions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/payment_institutions/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.payment_institution import PaymentInstitution
 from ...types.payments_institutions_paginated_response import PaymentsInstitutionsPaginatedResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 
 
 class PaymentInstitutionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_payment_institutions(
         self,
         *,
         page: typing.Optional[int] = None,
         country: typing.Optional[str] = None,
         country_in: typing.Optional[str] = None,
@@ -46,16 +48,16 @@
                 "created_at": created_at,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsInstitutionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -67,16 +69,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detail_payment_institution(self, id: str) -> PaymentInstitution:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"payments/institutions/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentInstitution, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -88,18 +90,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPaymentInstitutionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_payment_institutions(
         self,
         *,
         page: typing.Optional[int] = None,
         country: typing.Optional[str] = None,
         country_in: typing.Optional[str] = None,
@@ -121,16 +125,16 @@
                     "created_at": created_at,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsInstitutionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -143,16 +147,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detail_payment_institution(self, id: str) -> PaymentInstitution:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"payments/institutions/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentInstitution, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/payment_intents/client.py` & `fern_belvo-0.0.24/src/belvo/resources/tax_returns/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,109 +12,119 @@
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.create_payment_intent_pse import CreatePaymentIntentPse
+from ...types.detail_tax_return_response import DetailTaxReturnResponse
+from ...types.list_tax_returns_response import ListTaxReturnsResponse
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.patch_payment_intents_body_pse import PatchPaymentIntentsBodyPse
-from ...types.payment_intent_paginated_response import PaymentIntentPaginatedResponse
-from ...types.payment_intent_pse import PaymentIntentPse
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
+from ...types.retrieve_tax_returns_request_body import RetrieveTaxReturnsRequestBody
+from ...types.retrieve_tax_returns_response_item import RetrieveTaxReturnsResponseItem
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class PaymentIntentsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class TaxReturnsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_payment_intents(
+    def list_tax_returns(
         self,
         *,
         page: typing.Optional[int] = None,
-        id_in: typing.Optional[str] = None,
-        created_at: typing.Optional[str] = None,
+        page_size: typing.Optional[int] = None,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        link: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        provider: typing.Optional[str] = None,
-        payment_method_type: typing.Optional[str] = None,
-        customer: typing.Optional[str] = None,
-        customer_in: typing.Optional[str] = None,
-        amount: typing.Optional[str] = None,
-        amount_gt: typing.Optional[str] = None,
-        amount_gte: typing.Optional[str] = None,
-        amount_lt: typing.Optional[str] = None,
-        amount_lte: typing.Optional[str] = None,
-        status: typing.Optional[str] = None,
-        status_in: typing.Optional[str] = None,
-    ) -> PaymentIntentPaginatedResponse:
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        ejercicio: typing.Optional[str] = None,
+        ejercicio_lt: typing.Optional[str] = None,
+        ejercicio_lte: typing.Optional[str] = None,
+        ejercicio_gt: typing.Optional[str] = None,
+        ejercicio_gte: typing.Optional[str] = None,
+        ejercicio_range: typing.Optional[str] = None,
+        tipo_declaracion: typing.Optional[str] = None,
+        tipo_declaracion_in: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+    ) -> ListTaxReturnsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-returns"),
             params={
                 "page": page,
-                "id__in": id_in,
-                "created_at": created_at,
+                "page_size": page_size,
+                "omit": omit,
+                "fields": fields,
+                "link": link,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
-                "provider": provider,
-                "payment_method_type": payment_method_type,
-                "customer": customer,
-                "customer__in": customer_in,
-                "amount": amount,
-                "amount__gt": amount_gt,
-                "amount__gte": amount_gte,
-                "amount__lt": amount_lt,
-                "amount__lte": amount_lte,
-                "status": status,
-                "status__in": status_in,
+                "id": id,
+                "id__in": id_in,
+                "ejercicio": ejercicio,
+                "ejercicio__lt": ejercicio_lt,
+                "ejercicio__lte": ejercicio_lte,
+                "ejercicio__gt": ejercicio_gt,
+                "ejercicio__gte": ejercicio_gte,
+                "ejercicio__range": ejercicio_range,
+                "tipo_declaracion": tipo_declaracion,
+                "tipo_declaracion__in": tipo_declaracion_in,
+                "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListTaxReturnsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_payment_intent(self, *, request: CreatePaymentIntentPse) -> PaymentIntentPse:
+    def retrieve_tax_returns(
+        self,
+        *,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        request: RetrieveTaxReturnsRequestBody,
+    ) -> typing.List[RetrieveTaxReturnsResponseItem]:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-returns"),
+            params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RetrieveTaxReturnsResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -129,151 +139,161 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_payment_intent(self, id: str) -> PaymentIntentPse:
+    def detail_tax_return(
+        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
+    ) -> DetailTaxReturnResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-returns/{id}"),
+            params={"omit": omit, "fields": fields},
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxReturnResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def patch_payment_intent(
-        self, id: str, *, payment_method_details: PatchPaymentIntentsBodyPse, confirm: typing.Optional[bool] = OMIT
-    ) -> PaymentIntentPse:
-        _request: typing.Dict[str, typing.Any] = {"payment_method_details": payment_method_details}
-        if confirm is not OMIT:
-            _request["confirm"] = confirm
+    def destroy_tax_return(self, id: str) -> None:
         _response = httpx.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
-            json=jsonable_encoder(_request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-returns/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(
-                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
+            return
+        if _response.status_code == 401:
+            raise UnauthorizedError(
+                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncPaymentIntentsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncTaxReturnsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_payment_intents(
+    async def list_tax_returns(
         self,
         *,
         page: typing.Optional[int] = None,
-        id_in: typing.Optional[str] = None,
-        created_at: typing.Optional[str] = None,
+        page_size: typing.Optional[int] = None,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        link: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        provider: typing.Optional[str] = None,
-        payment_method_type: typing.Optional[str] = None,
-        customer: typing.Optional[str] = None,
-        customer_in: typing.Optional[str] = None,
-        amount: typing.Optional[str] = None,
-        amount_gt: typing.Optional[str] = None,
-        amount_gte: typing.Optional[str] = None,
-        amount_lt: typing.Optional[str] = None,
-        amount_lte: typing.Optional[str] = None,
-        status: typing.Optional[str] = None,
-        status_in: typing.Optional[str] = None,
-    ) -> PaymentIntentPaginatedResponse:
+        id: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        ejercicio: typing.Optional[str] = None,
+        ejercicio_lt: typing.Optional[str] = None,
+        ejercicio_lte: typing.Optional[str] = None,
+        ejercicio_gt: typing.Optional[str] = None,
+        ejercicio_gte: typing.Optional[str] = None,
+        ejercicio_range: typing.Optional[str] = None,
+        tipo_declaracion: typing.Optional[str] = None,
+        tipo_declaracion_in: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+    ) -> ListTaxReturnsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-returns"),
                 params={
                     "page": page,
-                    "id__in": id_in,
-                    "created_at": created_at,
+                    "page_size": page_size,
+                    "omit": omit,
+                    "fields": fields,
+                    "link": link,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
-                    "provider": provider,
-                    "payment_method_type": payment_method_type,
-                    "customer": customer,
-                    "customer__in": customer_in,
-                    "amount": amount,
-                    "amount__gt": amount_gt,
-                    "amount__gte": amount_gte,
-                    "amount__lt": amount_lt,
-                    "amount__lte": amount_lte,
-                    "status": status,
-                    "status__in": status_in,
+                    "id": id,
+                    "id__in": id_in,
+                    "ejercicio": ejercicio,
+                    "ejercicio__lt": ejercicio_lt,
+                    "ejercicio__lte": ejercicio_lte,
+                    "ejercicio__gt": ejercicio_gt,
+                    "ejercicio__gte": ejercicio_gte,
+                    "ejercicio__range": ejercicio_range,
+                    "tipo_declaracion": tipo_declaracion,
+                    "tipo_declaracion__in": tipo_declaracion_in,
+                    "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListTaxReturnsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_payment_intent(self, *, request: CreatePaymentIntentPse) -> PaymentIntentPse:
+    async def retrieve_tax_returns(
+        self,
+        *,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        request: RetrieveTaxReturnsRequestBody,
+    ) -> typing.List[RetrieveTaxReturnsResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-returns"),
+                params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RetrieveTaxReturnsResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -288,59 +308,56 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_payment_intent(self, id: str) -> PaymentIntentPse:
+    async def detail_tax_return(
+        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
+    ) -> DetailTaxReturnResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-returns/{id}"),
+                params={"omit": omit, "fields": fields},
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxReturnResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def patch_payment_intent(
-        self, id: str, *, payment_method_details: PatchPaymentIntentsBodyPse, confirm: typing.Optional[bool] = OMIT
-    ) -> PaymentIntentPse:
-        _request: typing.Dict[str, typing.Any] = {"payment_method_details": payment_method_details}
-        if confirm is not OMIT:
-            _request["confirm"] = confirm
+    async def destroy_tax_return(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
-                json=jsonable_encoder(_request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-returns/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(
-                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
+            return
+        if _response.status_code == 401:
+            raise UnauthorizedError(
+                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/payment_links/client.py` & `fern_belvo-0.0.24/src/belvo/resources/bank_accounts/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,92 +12,100 @@
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.create_paymentlink_request import CreatePaymentlinkRequest
-from ...types.create_paymentlink_response import CreatePaymentlinkResponse
-from ...types.detail_create_paymentlink_response import DetailCreatePaymentlinkResponse
-from ...types.list_payment_links_request_ordering import ListPaymentLinksRequestOrdering
-from ...types.list_payment_links_request_status import ListPaymentLinksRequestStatus
+from ...types.bank_account_paginated_response import BankAccountPaginatedResponse
+from ...types.create_bank_account_request import CreateBankAccountRequest
+from ...types.create_bank_account_response import CreateBankAccountResponse
+from ...types.detail_bank_account_response import DetailBankAccountResponse
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.payment_link_paginated_response import PaymentLinkPaginatedResponse
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class PaymentLinksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class BankAccountsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_payment_links(
+    def list_bank_account(
         self,
         *,
         page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        status: typing.Optional[ListPaymentLinksRequestStatus] = None,
-        ordering: typing.Optional[ListPaymentLinksRequestOrdering] = None,
-        search: typing.Optional[str] = None,
-    ) -> PaymentLinkPaginatedResponse:
+        number: typing.Optional[str] = None,
+        number_in: typing.Optional[str] = None,
+        customer: typing.Optional[str] = None,
+        institution: typing.Optional[str] = None,
+        holder_type: typing.Optional[str] = None,
+        holder_type_in: typing.Optional[str] = None,
+        providers: typing.Optional[str] = None,
+    ) -> BankAccountPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
             params={
                 "page": page,
-                "page_size": page_size,
+                "id__in": id_in,
                 "created_at": created_at,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
-                "status": status,
-                "ordering": ordering,
-                "search": search,
+                "number": number,
+                "number__in": number_in,
+                "customer": customer,
+                "institution": institution,
+                "holder__type": holder_type,
+                "holder__type__in": holder_type_in,
+                "providers": providers,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentLinkPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BankAccountPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_paymentlink(self, *, request: CreatePaymentlinkRequest) -> CreatePaymentlinkResponse:
+    def create_bank_account(self, *, request: CreateBankAccountRequest) -> CreateBankAccountResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreatePaymentlinkResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateBankAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -112,106 +120,116 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_create_paymentlink(self, access_token: str) -> DetailCreatePaymentlinkResponse:
+    def detail_bank_account(self, id: str) -> DetailBankAccountResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-links/{access_token}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/bank-accounts/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailCreatePaymentlinkResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailBankAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncPaymentLinksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncBankAccountsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_payment_links(
+    async def list_bank_account(
         self,
         *,
         page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        status: typing.Optional[ListPaymentLinksRequestStatus] = None,
-        ordering: typing.Optional[ListPaymentLinksRequestOrdering] = None,
-        search: typing.Optional[str] = None,
-    ) -> PaymentLinkPaginatedResponse:
+        number: typing.Optional[str] = None,
+        number_in: typing.Optional[str] = None,
+        customer: typing.Optional[str] = None,
+        institution: typing.Optional[str] = None,
+        holder_type: typing.Optional[str] = None,
+        holder_type_in: typing.Optional[str] = None,
+        providers: typing.Optional[str] = None,
+    ) -> BankAccountPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
                 params={
                     "page": page,
-                    "page_size": page_size,
+                    "id__in": id_in,
                     "created_at": created_at,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
-                    "status": status,
-                    "ordering": ordering,
-                    "search": search,
+                    "number": number,
+                    "number__in": number_in,
+                    "customer": customer,
+                    "institution": institution,
+                    "holder__type": holder_type,
+                    "holder__type__in": holder_type_in,
+                    "providers": providers,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentLinkPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BankAccountPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_paymentlink(self, *, request: CreatePaymentlinkRequest) -> CreatePaymentlinkResponse:
+    async def create_bank_account(self, *, request: CreateBankAccountRequest) -> CreateBankAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-links"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/bank-accounts"),
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreatePaymentlinkResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateBankAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -226,26 +244,26 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_create_paymentlink(self, access_token: str) -> DetailCreatePaymentlinkResponse:
+    async def detail_bank_account(self, id: str) -> DetailBankAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-links/{access_token}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/bank-accounts/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailCreatePaymentlinkResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailBankAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/payment_transactions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/payment_transactions/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.payment_transaction import PaymentTransaction
 from ...types.payments_transactions_paginated_response import PaymentsTransactionsPaginatedResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 
 
 class PaymentTransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_payment_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
@@ -74,16 +76,16 @@
                 "amount": amount,
                 "amount__gt": amount_gt,
                 "amount__gte": amount_gte,
                 "amount__lt": amount_lt,
                 "amount__lte": amount_lte,
                 "amount__range": amount_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsTransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -95,16 +97,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detail_payment_transactions(self, id: str) -> PaymentTransaction:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"payments/transactions/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentTransaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -116,18 +118,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPaymentTransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_payment_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         id_in: typing.Optional[str] = None,
         created_at: typing.Optional[str] = None,
@@ -177,16 +181,16 @@
                     "amount": amount,
                     "amount__gt": amount_gt,
                     "amount__gte": amount_gte,
                     "amount__lt": amount_lt,
                     "amount__lte": amount_lte,
                     "amount__range": amount_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsTransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -199,16 +203,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detail_payment_transactions(self, id: str) -> PaymentTransaction:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"payments/transactions/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentTransaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/payment_webhooks/client.py` & `fern_belvo-0.0.24/src/belvo/resources/payment_webhooks/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 from ...types.unexpected_error import UnexpectedError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class PaymentWebhooksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_payment_webhooks(self) -> PaymentsWebhooksPaginatedResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "payments/webhooks"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsWebhooksPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -62,16 +64,16 @@
             _request["auth_header"] = auth_header
         if auth_token is not OMIT:
             _request["auth_token"] = auth_token
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "payments/webhooks"),
             json=jsonable_encoder(_request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PaymentWebhook], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -95,16 +97,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detail_payment_webhooks(self, id: str) -> PaymentWebhook:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"payments/webhooks/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentWebhook, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -118,16 +120,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_payment_webhooks(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"payments/webhooks/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -139,26 +141,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPaymentWebhooksClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_payment_webhooks(self) -> PaymentsWebhooksPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "payments/webhooks"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentsWebhooksPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -179,16 +183,16 @@
         if auth_token is not OMIT:
             _request["auth_token"] = auth_token
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "payments/webhooks"),
                 json=jsonable_encoder(_request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PaymentWebhook], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -213,16 +217,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detail_payment_webhooks(self, id: str) -> PaymentWebhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"payments/webhooks/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentWebhook, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -237,16 +241,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_payment_webhooks(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"payments/webhooks/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/receivable_transactions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/receivable_transactions/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 from ...types.receivables_transactions_paginated_response import ReceivablesTransactionsPaginatedResponse
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class ReceivableTransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_receivable_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -74,16 +76,16 @@
                 "value_date": value_date,
                 "value_date__gt": value_date_gt,
                 "value_date__gte": value_date_gte,
                 "value_date__lt": value_date_lt,
                 "value_date__lte": value_date_lte,
                 "value_date__range": value_date_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -103,16 +105,16 @@
         request: ReceivableTransactionRequest,
     ) -> ReceivablesTransaction:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "receivables/transactions"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransaction, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -139,16 +141,16 @@
     def detail_receivable_transaction(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> ReceivablesTransaction:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"receivables/transactions/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -162,16 +164,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_receivable_transaction(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"receivables/transactions/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -183,18 +185,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncReceivableTransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_receivable_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -236,16 +240,16 @@
                     "value_date": value_date,
                     "value_date__gt": value_date_gt,
                     "value_date__gte": value_date_gte,
                     "value_date__lt": value_date_lt,
                     "value_date__lte": value_date_lte,
                     "value_date__range": value_date_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -266,16 +270,16 @@
     ) -> ReceivablesTransaction:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "receivables/transactions"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransaction, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -303,16 +307,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> ReceivablesTransaction:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"receivables/transactions/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReceivablesTransaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -327,16 +331,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_receivable_transaction(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"receivables/transactions/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/recurring_expenses/client.py` & `fern_belvo-0.0.24/src/belvo/resources/recurring_expenses/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class RecurringExpensesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_recurring_expenses(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -59,16 +61,16 @@
                 "link": link,
                 "account": account,
                 "account_in": account_in,
                 "id": id,
                 "id__in": id_in,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RecurringExpensesPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -88,16 +90,16 @@
         request: RecurringExpensesRequest,
     ) -> typing.List[RecurringExpenses]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/recurring-expenses"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -129,16 +131,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
     ) -> typing.List[RecurringExpenses]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/recurring-expenses"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -169,16 +171,16 @@
     def detail_recurring_expense(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> typing.List[RecurringExpenses]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/recurring-expenses/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -192,16 +194,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_recurring_expense(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/recurring-expenses/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -213,18 +215,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncRecurringExpensesClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_recurring_expenses(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -248,16 +252,16 @@
                     "link": link,
                     "account": account,
                     "account_in": account_in,
                     "id": id,
                     "id__in": id_in,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RecurringExpensesPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -278,16 +282,16 @@
     ) -> typing.List[RecurringExpenses]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/recurring-expenses"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -320,16 +324,16 @@
     ) -> typing.List[RecurringExpenses]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/recurring-expenses"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -361,16 +365,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> typing.List[RecurringExpenses]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/recurring-expenses/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RecurringExpenses], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -385,16 +389,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_recurring_expense(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/recurring-expenses/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/risk_insights/client.py` & `fern_belvo-0.0.24/src/belvo/resources/tax_declarations/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,191 +9,168 @@
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
-from ...errors.precondition_error import PreconditionError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
+from ...types.detail_tax_declaration_response import DetailTaxDeclarationResponse
+from ...types.list_tax_declarations_response import ListTaxDeclarationsResponse
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.patch_body import PatchBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
-from ...types.risk_insights import RiskInsights
-from ...types.risk_insights_paginated_response import RiskInsightsPaginatedResponse
-from ...types.standard_request import StandardRequest
-from ...types.token_required_response import TokenRequiredResponse
+from ...types.retrieve_tax_declarations_response_item import RetrieveTaxDeclarationsResponseItem
+from ...types.tax_declarations_request import TaxDeclarationsRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class RiskInsightsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class TaxDeclarationsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_risk_insights(
+    def list_tax_declarations(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
-    ) -> RiskInsightsPaginatedResponse:
+        year: typing.Optional[str] = None,
+        year_gt: typing.Optional[str] = None,
+        year_gte: typing.Optional[str] = None,
+        year_lt: typing.Optional[str] = None,
+        year_lte: typing.Optional[str] = None,
+        year_range: typing.Optional[str] = None,
+    ) -> ListTaxDeclarationsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
             params={
                 "page": page,
                 "page_size": page_size,
                 "omit": omit,
                 "fields": fields,
                 "link": link,
+                "link__in": link_in,
+                "created_at__gt": created_at_gt,
+                "created_at__gte": created_at_gte,
+                "created_at__lt": created_at_lt,
+                "created_at__lte": created_at_lte,
+                "created_at__range": created_at_range,
                 "id": id,
                 "id__in": id_in,
-                "link__in": link_in,
+                "year": year,
+                "year__gt": year_gt,
+                "year__gte": year_gte,
+                "year__lt": year_lt,
+                "year__lte": year_lte,
+                "year__range": year_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RiskInsightsPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListTaxDeclarationsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_risk_insights(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[RiskInsights]:
+    def retrieve_tax_declarations(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxDeclarationsRequest
+    ) -> typing.List[RetrieveTaxDeclarationsResponseItem]:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
-            params={"omit": omit, "fields": fields},
-            json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
-            else None,
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(
-                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
-            )
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
-            )
-        if _response.status_code == 408:
-            raise RequestTimeoutError(
-                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
-            )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
-        if _response.status_code == 500:
-            raise InternalServerError(
-                pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def patch_risk_insights(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[RiskInsights]:
-        _response = httpx.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RetrieveTaxDeclarationsResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_risk_insights(
+    def detail_tax_declaration(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> typing.List[RiskInsights]:
+    ) -> DetailTaxDeclarationResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxDeclarationResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_risk_insights(self, id: str) -> None:
+    def destroy_tax_declaration(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -204,181 +181,159 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncRiskInsightsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncTaxDeclarationsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_risk_insights(
+    async def list_tax_declarations(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
+        link_in: typing.Optional[str] = None,
+        created_at_gt: typing.Optional[str] = None,
+        created_at_gte: typing.Optional[str] = None,
+        created_at_lt: typing.Optional[str] = None,
+        created_at_lte: typing.Optional[str] = None,
+        created_at_range: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
-    ) -> RiskInsightsPaginatedResponse:
+        year: typing.Optional[str] = None,
+        year_gt: typing.Optional[str] = None,
+        year_gte: typing.Optional[str] = None,
+        year_lt: typing.Optional[str] = None,
+        year_lte: typing.Optional[str] = None,
+        year_range: typing.Optional[str] = None,
+    ) -> ListTaxDeclarationsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
                 params={
                     "page": page,
                     "page_size": page_size,
                     "omit": omit,
                     "fields": fields,
                     "link": link,
+                    "link__in": link_in,
+                    "created_at__gt": created_at_gt,
+                    "created_at__gte": created_at_gte,
+                    "created_at__lt": created_at_lt,
+                    "created_at__lte": created_at_lte,
+                    "created_at__range": created_at_range,
                     "id": id,
                     "id__in": id_in,
-                    "link__in": link_in,
+                    "year": year,
+                    "year__gt": year_gt,
+                    "year__gte": year_gte,
+                    "year__lt": year_lt,
+                    "year__lte": year_lte,
+                    "year__range": year_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RiskInsightsPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListTaxDeclarationsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_risk_insights(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[RiskInsights]:
+    async def retrieve_tax_declarations(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxDeclarationsRequest
+    ) -> typing.List[RetrieveTaxDeclarationsResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[RetrieveTaxDeclarationsResponseItem], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
-        if _response.status_code == 500:
-            raise InternalServerError(
-                pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def patch_risk_insights(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[RiskInsights]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/risk-insights"),
-                params={"omit": omit, "fields": fields},
-                json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
-                else None,
-                timeout=60,
-            )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(
-                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
-            )
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
-            )
-        if _response.status_code == 408:
-            raise RequestTimeoutError(
-                pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
-            )
-        if _response.status_code == 428:
-            raise PreconditionError(
-                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
-            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_risk_insights(
+    async def detail_tax_declaration(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> typing.List[RiskInsights]:
+    ) -> DetailTaxDeclarationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RiskInsights], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxDeclarationResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_risk_insights(self, id: str) -> None:
+    async def destroy_tax_declaration(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/risk-insights/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/secret_keys/client.py` & `fern_belvo-0.0.24/src/belvo/resources/secret_keys/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
 from ...types.secret_keys import SecretKeys
 from ...types.secret_keys_paginated_response import SecretKeysPaginatedResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 
 
 class SecretKeysClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_secret_keys(self) -> SecretKeysPaginatedResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "payments/secret-keys"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SecretKeysPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -46,16 +48,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_secret_keys(self) -> typing.List[SecretKeys]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "payments/secret-keys"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SecretKeys], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -69,26 +71,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncSecretKeysClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_secret_keys(self) -> SecretKeysPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "payments/secret-keys"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SecretKeysPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -101,16 +105,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_secret_keys(self) -> typing.List[SecretKeys]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "payments/secret-keys"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SecretKeys], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/tax_compliance_status/client.py` & `fern_belvo-0.0.24/src/belvo/resources/tax_status/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
+from ...types.detail_tax_status_response import DetailTaxStatusResponse
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
-from ...types.tax_compliance_status import TaxComplianceStatus
-from ...types.tax_compliance_status_paginated_response import TaxComplianceStatusPaginatedResponse
-from ...types.tax_compliance_status_request import TaxComplianceStatusRequest
+from ...types.retrieve_tax_status_response import RetrieveTaxStatusResponse
+from ...types.tax_status_paginated_response import TaxStatusPaginatedResponse
+from ...types.tax_status_request import TaxStatusRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class TaxComplianceStatusClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class TaxStatusClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_tax_compliance_status(
+    def list_tax_status(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
@@ -43,18 +46,18 @@
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> TaxComplianceStatusPaginatedResponse:
+    ) -> TaxStatusPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
             params={
                 "page": page,
                 "page_size": page_size,
                 "omit": omit,
                 "fields": fields,
                 "link": link,
                 "created_at__gt": created_at_gt,
@@ -62,50 +65,46 @@
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
                 "id": id,
                 "id__in": id_in,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatusPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxStatusPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_tax_compliance_status(
-        self,
-        *,
-        omit: typing.Optional[str] = None,
-        fields: typing.Optional[str] = None,
-        request: TaxComplianceStatusRequest,
-    ) -> TaxComplianceStatus:
+    def retrieve_tax_status(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxStatusRequest
+    ) -> RetrieveTaxStatusResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveTaxStatusResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -120,46 +119,46 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_tax_compliance_status(
+    def detail_tax_status(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> TaxComplianceStatus:
+    ) -> DetailTaxStatusResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxStatusResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_tax_compliance_status(self, id: str) -> None:
+    def destroy_tax_status(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -170,21 +169,23 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTaxComplianceStatusClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncTaxStatusClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_tax_compliance_status(
+    async def list_tax_status(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: typing.Optional[str] = None,
@@ -192,19 +193,19 @@
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
         id: typing.Optional[str] = None,
         id_in: typing.Optional[str] = None,
         link_in: typing.Optional[str] = None,
-    ) -> TaxComplianceStatusPaginatedResponse:
+    ) -> TaxStatusPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
                 params={
                     "page": page,
                     "page_size": page_size,
                     "omit": omit,
                     "fields": fields,
                     "link": link,
                     "created_at__gt": created_at_gt,
@@ -212,51 +213,47 @@
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
                     "id": id,
                     "id__in": id_in,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatusPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TaxStatusPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_tax_compliance_status(
-        self,
-        *,
-        omit: typing.Optional[str] = None,
-        fields: typing.Optional[str] = None,
-        request: TaxComplianceStatusRequest,
-    ) -> TaxComplianceStatus:
+    async def retrieve_tax_status(
+        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxStatusRequest
+    ) -> RetrieveTaxStatusResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-compliance-status"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveTaxStatusResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -271,48 +268,48 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_tax_compliance_status(
+    async def detail_tax_status(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> TaxComplianceStatus:
+    ) -> DetailTaxStatusResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxComplianceStatus, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DetailTaxStatusResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_tax_compliance_status(self, id: str) -> None:
+    async def destroy_tax_status(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-compliance-status/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/tax_declarations/client.py` & `fern_belvo-0.0.24/src/belvo/resources/payment_intents/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,109 +12,111 @@
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.detail_tax_declaration_response import DetailTaxDeclarationResponse
-from ...types.list_tax_declarations_response import ListTaxDeclarationsResponse
+from ...types.create_payment_intent_pse import CreatePaymentIntentPse
 from ...types.not_found_error_body import NotFoundErrorBody
+from ...types.patch_payment_intents_body_pse import PatchPaymentIntentsBodyPse
+from ...types.payment_intent_paginated_response import PaymentIntentPaginatedResponse
+from ...types.payment_intent_pse import PaymentIntentPse
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
-from ...types.retrieve_tax_declarations_response_item import RetrieveTaxDeclarationsResponseItem
-from ...types.tax_declarations_request import TaxDeclarationsRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
-class TaxDeclarationsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+
+class PaymentIntentsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_tax_declarations(
+    def list_payment_intents(
         self,
         *,
         page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
-        omit: typing.Optional[str] = None,
-        fields: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        id: typing.Optional[str] = None,
-        id_in: typing.Optional[str] = None,
-        year: typing.Optional[str] = None,
-        year_gt: typing.Optional[str] = None,
-        year_gte: typing.Optional[str] = None,
-        year_lt: typing.Optional[str] = None,
-        year_lte: typing.Optional[str] = None,
-        year_range: typing.Optional[str] = None,
-    ) -> ListTaxDeclarationsResponse:
+        provider: typing.Optional[str] = None,
+        payment_method_type: typing.Optional[str] = None,
+        customer: typing.Optional[str] = None,
+        customer_in: typing.Optional[str] = None,
+        amount: typing.Optional[str] = None,
+        amount_gt: typing.Optional[str] = None,
+        amount_gte: typing.Optional[str] = None,
+        amount_lt: typing.Optional[str] = None,
+        amount_lte: typing.Optional[str] = None,
+        status: typing.Optional[str] = None,
+        status_in: typing.Optional[str] = None,
+    ) -> PaymentIntentPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
             params={
                 "page": page,
-                "page_size": page_size,
-                "omit": omit,
-                "fields": fields,
-                "link": link,
-                "link__in": link_in,
+                "id__in": id_in,
+                "created_at": created_at,
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
-                "id": id,
-                "id__in": id_in,
-                "year": year,
-                "year__gt": year_gt,
-                "year__gte": year_gte,
-                "year__lt": year_lt,
-                "year__lte": year_lte,
-                "year__range": year_range,
+                "provider": provider,
+                "payment_method_type": payment_method_type,
+                "customer": customer,
+                "customer__in": customer_in,
+                "amount": amount,
+                "amount__gt": amount_gt,
+                "amount__gte": amount_gte,
+                "amount__lt": amount_lt,
+                "amount__lte": amount_lte,
+                "status": status,
+                "status__in": status_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListTaxDeclarationsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_tax_declarations(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxDeclarationsRequest
-    ) -> typing.List[RetrieveTaxDeclarationsResponseItem]:
+    def create_payment_intent(self, *, request: CreatePaymentIntentPse) -> PaymentIntentPse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
-            params={"omit": omit, "fields": fields},
+            urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RetrieveTaxDeclarationsResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -129,151 +131,153 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_tax_declaration(
-        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> DetailTaxDeclarationResponse:
+    def detail_payment_intent(self, id: str) -> PaymentIntentPse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
-            params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailTaxDeclarationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_tax_declaration(self, id: str) -> None:
+    def patch_payment_intent(
+        self, id: str, *, payment_method_details: PatchPaymentIntentsBodyPse, confirm: typing.Optional[bool] = OMIT
+    ) -> PaymentIntentPse:
+        _request: typing.Dict[str, typing.Any] = {"payment_method_details": payment_method_details}
+        if confirm is not OMIT:
+            _request["confirm"] = confirm
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
+            json=jsonable_encoder(_request),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTaxDeclarationsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncPaymentIntentsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_tax_declarations(
+    async def list_payment_intents(
         self,
         *,
         page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
-        omit: typing.Optional[str] = None,
-        fields: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
+        id_in: typing.Optional[str] = None,
+        created_at: typing.Optional[str] = None,
         created_at_gt: typing.Optional[str] = None,
         created_at_gte: typing.Optional[str] = None,
         created_at_lt: typing.Optional[str] = None,
         created_at_lte: typing.Optional[str] = None,
         created_at_range: typing.Optional[str] = None,
-        id: typing.Optional[str] = None,
-        id_in: typing.Optional[str] = None,
-        year: typing.Optional[str] = None,
-        year_gt: typing.Optional[str] = None,
-        year_gte: typing.Optional[str] = None,
-        year_lt: typing.Optional[str] = None,
-        year_lte: typing.Optional[str] = None,
-        year_range: typing.Optional[str] = None,
-    ) -> ListTaxDeclarationsResponse:
+        provider: typing.Optional[str] = None,
+        payment_method_type: typing.Optional[str] = None,
+        customer: typing.Optional[str] = None,
+        customer_in: typing.Optional[str] = None,
+        amount: typing.Optional[str] = None,
+        amount_gt: typing.Optional[str] = None,
+        amount_gte: typing.Optional[str] = None,
+        amount_lt: typing.Optional[str] = None,
+        amount_lte: typing.Optional[str] = None,
+        status: typing.Optional[str] = None,
+        status_in: typing.Optional[str] = None,
+    ) -> PaymentIntentPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
                 params={
                     "page": page,
-                    "page_size": page_size,
-                    "omit": omit,
-                    "fields": fields,
-                    "link": link,
-                    "link__in": link_in,
+                    "id__in": id_in,
+                    "created_at": created_at,
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
-                    "id": id,
-                    "id__in": id_in,
-                    "year": year,
-                    "year__gt": year_gt,
-                    "year__gte": year_gte,
-                    "year__lt": year_lt,
-                    "year__lte": year_lte,
-                    "year__range": year_range,
+                    "provider": provider,
+                    "payment_method_type": payment_method_type,
+                    "customer": customer,
+                    "customer__in": customer_in,
+                    "amount": amount,
+                    "amount__gt": amount_gt,
+                    "amount__gte": amount_gte,
+                    "amount__lt": amount_lt,
+                    "amount__lte": amount_lte,
+                    "status": status,
+                    "status__in": status_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListTaxDeclarationsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_tax_declarations(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxDeclarationsRequest
-    ) -> typing.List[RetrieveTaxDeclarationsResponseItem]:
+    async def create_payment_intent(self, *, request: CreatePaymentIntentPse) -> PaymentIntentPse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-declarations"),
-                params={"omit": omit, "fields": fields},
+                urllib.parse.urljoin(f"{self._environment.value}/", "payments/payment-intents"),
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[RetrieveTaxDeclarationsResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -288,56 +292,59 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_tax_declaration(
-        self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> DetailTaxDeclarationResponse:
+    async def detail_payment_intent(self, id: str) -> PaymentIntentPse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
-                params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailTaxDeclarationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_tax_declaration(self, id: str) -> None:
+    async def patch_payment_intent(
+        self, id: str, *, payment_method_details: PatchPaymentIntentsBodyPse, confirm: typing.Optional[bool] = OMIT
+    ) -> PaymentIntentPse:
+        _request: typing.Dict[str, typing.Any] = {"payment_method_details": payment_method_details}
+        if confirm is not OMIT:
+            _request["confirm"] = confirm
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-declarations/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                "PATCH",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"payments/payment-intents/{id}"),
+                json=jsonable_encoder(_request),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaymentIntentPse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/tax_retentions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/tax_retentions/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 from ...types.tax_retentions_paginated_response import TaxRetentionsPaginatedResponse
 from ...types.tax_retentions_request import TaxRetentionsRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class TaxRetentionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_tax_retentions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -58,16 +60,16 @@
                 "created_at__gt": created_at_gt,
                 "created_at__gte": created_at_gte,
                 "created_at__lt": created_at_lt,
                 "created_at__lte": created_at_lte,
                 "created_at__range": created_at_range,
                 "link__in": link_in,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRetentionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -83,16 +85,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxRetentionsRequest
     ) -> typing.List[TaxRetentions]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-retentions"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[TaxRetentions], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -119,16 +121,16 @@
     def detail_tax_retentions(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> TaxRetentions:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-retentions/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRetentions, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -142,16 +144,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_tax_retention(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-retentions/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -163,18 +165,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTaxRetentionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_tax_retentions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -200,16 +204,16 @@
                     "created_at__gt": created_at_gt,
                     "created_at__gte": created_at_gte,
                     "created_at__lt": created_at_lt,
                     "created_at__lte": created_at_lte,
                     "created_at__range": created_at_range,
                     "link__in": link_in,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRetentionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -226,16 +230,16 @@
     ) -> typing.List[TaxRetentions]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-retentions"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[TaxRetentions], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -263,16 +267,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> TaxRetentions:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-retentions/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRetentions, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -287,16 +291,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_tax_retention(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-retentions/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/tax_status/client.py` & `fern_belvo-0.0.24/src/belvo/resources/employment_records/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,154 +9,142 @@
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...environment import BelvoEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
+from ...errors.precondition_error import PreconditionError
 from ...errors.request_timeout_error import RequestTimeoutError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.bad_request_error_body_item import BadRequestErrorBodyItem
-from ...types.detail_tax_status_response import DetailTaxStatusResponse
+from ...types.employment_record import EmploymentRecord
+from ...types.employment_record_request import EmploymentRecordRequest
+from ...types.employment_records_paginated_response import EmploymentRecordsPaginatedResponse
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.request_timeout_error_body import RequestTimeoutErrorBody
-from ...types.retrieve_tax_status_response import RetrieveTaxStatusResponse
-from ...types.tax_status_paginated_response import TaxStatusPaginatedResponse
-from ...types.tax_status_request import TaxStatusRequest
+from ...types.token_required_response import TokenRequiredResponse
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
-class TaxStatusClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class EmploymentRecordsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    def list_tax_status(
+    def list_employment_records(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
-        created_at_gt: typing.Optional[str] = None,
-        created_at_gte: typing.Optional[str] = None,
-        created_at_lt: typing.Optional[str] = None,
-        created_at_lte: typing.Optional[str] = None,
-        created_at_range: typing.Optional[str] = None,
-        id: typing.Optional[str] = None,
-        id_in: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
-    ) -> TaxStatusPaginatedResponse:
+    ) -> EmploymentRecordsPaginatedResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
-            params={
-                "page": page,
-                "page_size": page_size,
-                "omit": omit,
-                "fields": fields,
-                "link": link,
-                "created_at__gt": created_at_gt,
-                "created_at__gte": created_at_gte,
-                "created_at__lt": created_at_lt,
-                "created_at__lte": created_at_lte,
-                "created_at__range": created_at_range,
-                "id": id,
-                "id__in": id_in,
-                "link__in": link_in,
-            },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
+            params={"page": page, "page_size": page_size, "omit": omit, "fields": fields},
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxStatusPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EmploymentRecordsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_tax_status(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxStatusRequest
-    ) -> RetrieveTaxStatusResponse:
+    def retrieve_employment_record_details(
+        self,
+        *,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        request: EmploymentRecordRequest,
+    ) -> typing.List[EmploymentRecord]:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RetrieveTaxStatusResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EmploymentRecord], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
+        if _response.status_code == 428:
+            raise PreconditionError(
+                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
+            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def detail_tax_status(
+    def detail_employment_record(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> DetailTaxStatusResponse:
+    ) -> EmploymentRecord:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailTaxStatusResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EmploymentRecord, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy_tax_status(self, id: str) -> None:
+    def destroy_employment_record(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -167,145 +155,132 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTaxStatusClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+class AsyncEmploymentRecordsClient:
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
-    async def list_tax_status(
+    async def list_employment_records(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
-        link: typing.Optional[str] = None,
-        created_at_gt: typing.Optional[str] = None,
-        created_at_gte: typing.Optional[str] = None,
-        created_at_lt: typing.Optional[str] = None,
-        created_at_lte: typing.Optional[str] = None,
-        created_at_range: typing.Optional[str] = None,
-        id: typing.Optional[str] = None,
-        id_in: typing.Optional[str] = None,
-        link_in: typing.Optional[str] = None,
-    ) -> TaxStatusPaginatedResponse:
+    ) -> EmploymentRecordsPaginatedResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
-                params={
-                    "page": page,
-                    "page_size": page_size,
-                    "omit": omit,
-                    "fields": fields,
-                    "link": link,
-                    "created_at__gt": created_at_gt,
-                    "created_at__gte": created_at_gte,
-                    "created_at__lt": created_at_lt,
-                    "created_at__lte": created_at_lte,
-                    "created_at__range": created_at_range,
-                    "id": id,
-                    "id__in": id_in,
-                    "link__in": link_in,
-                },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
+                params={"page": page, "page_size": page_size, "omit": omit, "fields": fields},
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TaxStatusPaginatedResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EmploymentRecordsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_tax_status(
-        self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TaxStatusRequest
-    ) -> RetrieveTaxStatusResponse:
+    async def retrieve_employment_record_details(
+        self,
+        *,
+        omit: typing.Optional[str] = None,
+        fields: typing.Optional[str] = None,
+        request: EmploymentRecordRequest,
+    ) -> typing.List[EmploymentRecord]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/tax-status"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/employment-records"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RetrieveTaxStatusResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EmploymentRecord], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 408:
             raise RequestTimeoutError(
                 pydantic.parse_obj_as(typing.List[RequestTimeoutErrorBody], _response.json())  # type: ignore
             )
+        if _response.status_code == 428:
+            raise PreconditionError(
+                pydantic.parse_obj_as(typing.List[TokenRequiredResponse], _response.json())  # type: ignore
+            )
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic.parse_obj_as(typing.List[UnexpectedError], _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def detail_tax_status(
+    async def detail_employment_record(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> DetailTaxStatusResponse:
+    ) -> EmploymentRecord:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DetailTaxStatusResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EmploymentRecord, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy_tax_status(self, id: str) -> None:
+    async def destroy_employment_record(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/tax-status/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/employment-records/{id}"),
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/resources/transactions/client.py` & `fern_belvo-0.0.24/src/belvo/resources/transactions/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 from ...types.transactions_paginated_response import TransactionsPaginatedResponse
 from ...types.transactions_request import TransactionsRequest
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from ...types.unexpected_error import UnexpectedError
 
 
 class TransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     def list_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -157,16 +159,16 @@
                 "value_date": value_date,
                 "value_date__gt": value_date_gt,
                 "value_date__gte": value_date_gte,
                 "value_date__lt": value_date_lt,
                 "value_date__lte": value_date_lte,
                 "value_date__range": value_date_range,
             },
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -182,16 +184,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: TransactionsRequest
     ) -> typing.List[Transaction]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Transaction], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -224,16 +226,16 @@
     ) -> AsynchronousAccepted202:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers({"X-Belvo-Request-Mode": "async"}),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AsynchronousAccepted202, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -265,16 +267,16 @@
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
     ) -> typing.List[Transaction]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Transaction], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -305,16 +307,16 @@
     def detail_transaction(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Transaction:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/transactions/{id}"),
             params={"omit": omit, "fields": fields},
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Transaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -328,16 +330,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy_transaction(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/transactions/{id}"),
-            auth=(self._username, self._password)
-            if self._username is not None and self._password is not None
+            auth=(self._secret_id, self._secret_password)
+            if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -349,18 +351,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTransactionsClient:
-    def __init__(self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, username: str, password: str):
+    def __init__(
+        self, *, environment: BelvoEnvironment = BelvoEnvironment.PRODUCTION, secret_id: str, secret_password: str
+    ):
         self._environment = environment
-        self._username = username
-        self._password = password
+        self._secret_id = secret_id
+        self._secret_password = secret_password
 
     async def list_transactions(
         self,
         *,
         page: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         omit: typing.Optional[str] = None,
@@ -480,16 +484,16 @@
                     "value_date": value_date,
                     "value_date__gt": value_date_gt,
                     "value_date__gte": value_date_gte,
                     "value_date__lt": value_date_lt,
                     "value_date__lte": value_date_lte,
                     "value_date__range": value_date_range,
                 },
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TransactionsPaginatedResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -506,16 +510,16 @@
     ) -> typing.List[Transaction]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Transaction], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -549,16 +553,16 @@
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers({"X-Belvo-Request-Mode": "async"}),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AsynchronousAccepted202, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -591,16 +595,16 @@
     ) -> typing.List[Transaction]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/transactions"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Transaction], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
@@ -632,16 +636,16 @@
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
     ) -> Transaction:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/transactions/{id}"),
                 params={"omit": omit, "fields": fields},
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Transaction, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
@@ -656,16 +660,16 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy_transaction(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/transactions/{id}"),
-                auth=(self._username, self._password)
-                if self._username is not None and self._password is not None
+                auth=(self._secret_id, self._secret_password)
+                if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/__init__.py` & `fern_belvo-0.0.24/src/belvo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/access_to_resource_denied.py` & `fern_belvo-0.0.24/src/belvo/types/access_to_resource_denied.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`access_to_resource_denied`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#403-access_to_resource_denied" target="_blank">403 access_to_resource_denied</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `access_to_resource_denied` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `You don't have access to this resource.`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/account.py` & `fern_belvo-0.0.24/src/belvo/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_balance.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_balance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_credit_data.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_credit_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_funds_data.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_funds_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_funds_data_public_identifications.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_funds_data_public_identifications.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_loan_data.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_loan_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_loan_data_fees.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_loan_data_fees.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_loan_data_interest_rate.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_loan_data_interest_rate.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/accounts_receivables_data.py` & `fern_belvo-0.0.24/src/belvo/types/accounts_receivables_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/annual_costs_and_deductions_statement_business.py` & `fern_belvo-0.0.24/src/belvo/types/annual_costs_and_deductions_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/annual_income_statement_business.py` & `fern_belvo-0.0.24/src/belvo/types/annual_income_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/annual_income_statement_individual.py` & `fern_belvo-0.0.24/src/belvo/types/annual_income_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/annual_totals_individual.py` & `fern_belvo-0.0.24/src/belvo/types/annual_totals_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/asynchronous_accepted_202.py` & `fern_belvo-0.0.24/src/belvo/types/asynchronous_accepted_202.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bad_request_error_body_item.py` & `fern_belvo-0.0.24/src/belvo/types/bad_request_error_body_item.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/balance.py` & `fern_belvo-0.0.24/src/belvo/types/balance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/balances_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/balances_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/balances_request.py` & `fern_belvo-0.0.24/src/belvo/types/balances_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_business_pse.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_details_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_details_ofpi_pix.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_details_ofpi_pix.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_details_open_finance.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_details_open_finance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_details_open_finance_pix.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_details_open_finance_pix.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_holder_request_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_holder_request_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_information_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_information_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_information_pse.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_ofpi_response.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/bank_account_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/bank_account_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/beneficiary_bank_account_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/beneficiary_bank_account_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/beneficiary_bank_account_pse.py` & `fern_belvo-0.0.24/src/belvo/types/beneficiary_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/categorization.py` & `fern_belvo-0.0.24/src/belvo/types/categorization.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/categorization_body.py` & `fern_belvo-0.0.24/src/belvo/types/categorization_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/categorization_body_request.py` & `fern_belvo-0.0.24/src/belvo/types/categorization_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/categorization_merchant_data.py` & `fern_belvo-0.0.24/src/belvo/types/categorization_merchant_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/change_access_mode.py` & `fern_belvo-0.0.24/src/belvo/types/change_access_mode.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge.py` & `fern_belvo-0.0.24/src/belvo/types/charge.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_ofpi_content.py` & `fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_ofpi_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge_payment_method_details_pse_content.py` & `fern_belvo-0.0.24/src/belvo/types/charge_payment_method_details_pse_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/charge_status.py` & `fern_belvo-0.0.24/src/belvo/types/charge_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_bank_account_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/create_bank_account_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_bank_account_pse.py` & `fern_belvo-0.0.24/src/belvo/types/create_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_customer_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/create_customer_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_customer_pse.py` & `fern_belvo-0.0.24/src/belvo/types/create_customer_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_payment_intent_pse.py` & `fern_belvo-0.0.24/src/belvo/types/create_payment_intent_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_payment_link_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/create_payment_link_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/create_payment_link_pse.py` & `fern_belvo-0.0.24/src/belvo/types/create_payment_link_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/customer_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/customer_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/customer_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/customer_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/customer_pse.py` & `fern_belvo-0.0.24/src/belvo/types/customer_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_confirmation_required_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/display_confirmation_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_confirmation_required_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/display_confirmation_required_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_credentials_required_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/display_credentials_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_customer_bank_accounts_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/display_customer_bank_accounts_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_payment_failed.py` & `fern_belvo-0.0.24/src/belvo/types/display_payment_failed.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_payment_method_information_content_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/display_payment_method_information_content_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_payment_method_information_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/display_payment_method_information_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_payment_processing.py` & `fern_belvo-0.0.24/src/belvo/types/display_payment_processing.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_payment_succeeded.py` & `fern_belvo-0.0.24/src/belvo/types/display_payment_succeeded.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/display_token_required_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/display_token_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/document_id_business.py` & `fern_belvo-0.0.24/src/belvo/types/document_id_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/document_id_individual.py` & `fern_belvo-0.0.24/src/belvo/types/document_id_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/document_information_business.py` & `fern_belvo-0.0.24/src/belvo/types/document_information_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/document_information_individual.py` & `fern_belvo-0.0.24/src/belvo/types/document_information_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_detail.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_detail.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_document_id.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_document_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_employment_status_updates.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_employment_status_updates.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_entitlement.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_entitlement.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_file.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_file.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_personal_data.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_personal_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_request.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_record_social_security_summary.py` & `fern_belvo-0.0.24/src/belvo/types/employment_record_social_security_summary.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/employment_records_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/employment_records_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_bank_account_holder_type_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/enum_bank_account_holder_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_categorization_account_category.py` & `fern_belvo-0.0.24/src/belvo/types/enum_categorization_account_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_categorization_account_holder_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_categorization_account_holder_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_categorization_transaction_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_categorization_transaction_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_customer_identifier_type_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/enum_customer_identifier_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_customer_identifier_type_pse.py` & `fern_belvo-0.0.24/src/belvo/types/enum_customer_identifier_type_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_customer_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_customer_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_employment_record_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_employment_record_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_employment_record_status_update_events.py` & `fern_belvo-0.0.24/src/belvo/types/enum_employment_record_status_update_events.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_income_minimum_confidence_level_request.py` & `fern_belvo-0.0.24/src/belvo/types/enum_income_minimum_confidence_level_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_income_stream_confidence.py` & `fern_belvo-0.0.24/src/belvo/types/enum_income_stream_confidence.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_income_stream_frequency.py` & `fern_belvo-0.0.24/src/belvo/types/enum_income_stream_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_income_stream_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_income_stream_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_income_verification_account_category.py` & `fern_belvo-0.0.24/src/belvo/types/enum_income_verification_account_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_institution_integration_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_institution_integration_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_institution_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_institution_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_institution_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_institution_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_investment_portfolio_instrument_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_investment_portfolio_instrument_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_investment_portfolio_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_investment_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_invoice_allowed_income_types_request.py` & `fern_belvo-0.0.24/src/belvo/types/enum_invoice_allowed_income_types_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_invoice_sat_invoice_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_invoice_sat_invoice_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_link_access_mode_request.py` & `fern_belvo-0.0.24/src/belvo/types/enum_link_access_mode_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_link_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_link_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_loan_data_fee_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_loan_data_fee_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_loan_data_interest_rate_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_loan_data_interest_rate_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_intent_holder_type_pse.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_intent_holder_type_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_intent_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_intent_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_link_allowed_payment_method.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_link_allowed_payment_method.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_link_provider.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_link_provider.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_links_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_links_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payment_transaction_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payments_country.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payments_country.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_payments_currency.py` & `fern_belvo-0.0.24/src/belvo/types/enum_payments_currency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_receivable_transaction_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_receivable_transaction_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_category.py` & `fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_frequency.py` & `fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_recurring_expense_payment_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_recurring_expense_payment_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_tax_compliance_status_outcome.py` & `fern_belvo-0.0.24/src/belvo/types/enum_tax_compliance_status_outcome.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_payment_status.py` & `fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_payment_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_receiver_nationality.py` & `fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_receiver_nationality.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/enum_tax_retention_type.py` & `fern_belvo-0.0.24/src/belvo/types/enum_tax_retention_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/equity_statement_business.py` & `fern_belvo-0.0.24/src/belvo/types/equity_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/equity_statement_individual.py` & `fern_belvo-0.0.24/src/belvo/types/equity_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/eyod_income_verification_body_request.py` & `fern_belvo-0.0.24/src/belvo/types/eyod_income_verification_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/gross_income_individual.py` & `fern_belvo-0.0.24/src/belvo/types/gross_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_bank_account_information_pse.py` & `fern_belvo-0.0.24/src/belvo/types/holder_bank_account_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_bank_account_pse.py` & `fern_belvo-0.0.24/src/belvo/types/holder_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_business_pse.py` & `fern_belvo-0.0.24/src/belvo/types/holder_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_business_response_pse.py` & `fern_belvo-0.0.24/src/belvo/types/holder_business_response_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_business_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_business_ofpi_response.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_business_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_business_pse.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_business_pse_response.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_business_pse_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_individual_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_information_individual_ofpi_response.py` & `fern_belvo-0.0.24/src/belvo/types/holder_information_individual_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/holder_response_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/holder_response_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/income.py` & `fern_belvo-0.0.24/src/belvo/types/income.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/income_streams_body.py` & `fern_belvo-0.0.24/src/belvo/types/income_streams_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/incomes_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/incomes_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/incomes_request.py` & `fern_belvo-0.0.24/src/belvo/types/incomes_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution.py` & `fern_belvo-0.0.24/src/belvo/types/institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     resources: typing.Optional[typing.List[str]] = pydantic.Field(
         description=(
             "A list of Belvo resources that you can use with the institution. This list includes one or more of the following resources:\n"
             "\n"
             "  - `ACCOUNTS`\n"
             "  - `BALANCES`\n"
             "  - `INCOMES`\n"
-            "  - `INVESTMENTS_PORTFOLIOS` \n"
+            "  - `INVESTMENTS_PORTFOLIOS`\n"
             "  - `INVESTMENTS_TRANSACTIONS` *This field has been deprecated.*\n"
             "  - `INVOICES`\n"
             "  - `OWNERS`\n"
             "  - `RECURRING_EXPENSES`\n"
             "  - `RISK_INSIGHTS`\n"
             "  - `TRANSACTIONS`\n"
             "  - `TAX_COMPLIANCE_STATUS`\n"
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution_account.py` & `fern_belvo-0.0.24/src/belvo/types/institution_account.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution_down_error.py` & `fern_belvo-0.0.24/src/belvo/types/institution_down_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`institution_down`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-institution_down" target="_blank">400 institution_down errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `institution_down` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `The financial institution is down, try again later`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution_form_field.py` & `fern_belvo-0.0.24/src/belvo/types/institution_form_field.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution_inactive_error.py` & `fern_belvo-0.0.24/src/belvo/types/institution_inactive_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`institution_inactive`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-institution_inactive" target="_blank">400 institution_inactive errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `institution_inactive` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `The institution has been temporarily deactivated`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/institution_unavailable_error.py` & `fern_belvo-0.0.24/src/belvo/types/institution_unavailable_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
             "A short description of the error.\n"
             "\n"
             "For `institution_unavailable` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `The financial institution is unavailable`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/institutions_feature.py` & `fern_belvo-0.0.24/src/belvo/types/institutions_feature.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institutions_form_field.py` & `fern_belvo-0.0.24/src/belvo/types/institutions_form_field.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institutions_form_field_values.py` & `fern_belvo-0.0.24/src/belvo/types/institutions_form_field_values.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/institutions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/institutions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invalid_access_mode.py` & `fern_belvo-0.0.24/src/belvo/types/invalid_access_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`invalid_access_mode_switch`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-invalid_access_mode_switch" target="_blank">400 invalid_access_mode_switch errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `invalid_access_mode_switch` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `This link doesn't have stored credentials hence it can't be switched to recurrent mode\"`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invalid_link_error.py` & `fern_belvo-0.0.24/src/belvo/types/session_expired_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InvalidLinkError(pydantic.BaseModel):
+class SessionExpiredError(pydantic.BaseModel):
     """
-    This error occurs when you try to access an account but the user credentials are no longer valid, prompting an error from the institution.
+    This error occurs when you try to resume a request session that has already expired. This is usually because the user took too long to provide their authentication token.
     """
 
     code: typing.Optional[str] = pydantic.Field(
         description=(
-            "A unique error code (`invalid_link`) that allows you to classify and handle the error programmatically.\n"
+            "A unique error code (`session_expired`) that allows you to classify and handle the error programmatically.\n"
             "\n"
-            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-invalid_link" target="_blank">400 invalid_link errors</a>.\n'
+            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-session_expired" target="_blank">400 session_expired errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
-            "For `invalid_link` errors, the description is:\n"
-            "  \n"
-            "  - `The link has been invalidated. You may need to update link credentials`.\n"
+            "For `session_expired` errors, the description is:\n"
+            "\n"
+            "  - `The session you are trying to resume has expired, please start again from register/retrieve endpoint`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
     )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invalid_period_error.py` & `fern_belvo-0.0.24/src/belvo/types/invalid_period_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`invalid_period`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-invalid_period" target="_blank">400 invalid_period errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `invalid_period` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `The number of days between date_from and date_to must be at least 90 days`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_fees.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_fees.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_interest_rate.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_interest_rate.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_public_id.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_public_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/investments_portfolios_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/investments_portfolios_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_detail_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_detail_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_detail_retained_tax_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_detail_retained_tax_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_detail_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_detail_sat.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "The identification code of the product or the service, as defined by the legal entity in the country.\n"
             "- 🇲🇽 [Mexico](http://200.57.3.89/Pys/catPyS.aspx)\n"
         )
     )
     quantity: typing.Optional[int] = pydantic.Field(description=("The quantity of this invoice item.\n"))
     unit_code: typing.Optional[str] = pydantic.Field(
         description=(
-            "The unit of measure, as defined by the legal entity in the country. \n"
+            "The unit of measure, as defined by the legal entity in the country.\n"
             "- 🇲🇽 Mexico [SAT catalog reference](https://developers.belvo.com/docs/sat-catalogs#unit-code)\n"
         )
     )
     unit_description: typing.Optional[str] = pydantic.Field(
         description=(
             "The description of the item, as defined by the legal entity in the country.\n"
             "- 🇲🇽 Mexico [SAT catalog reference](https://developers.belvo.com/docs/sat-catalogs#unit-code)\n"
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_dian.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     )
     invoice_details: typing.List[InvoiceDetailDian] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     currency: typing.Optional[str] = pydantic.Field(
         description=(
             "The currency of the invoice. For example:\n"
-            " \n"
+            "\n"
             " - 🇧🇷 BRL (Brazilian Real)\n"
             " - 🇨🇴 COP (Colombian Peso)\n"
             " - 🇲🇽 MXN (Mexican Peso)\n"
             " - 🇺🇸 USD (United States Dollar)\n"
         )
     )
     subtotal_amount: typing.Optional[float] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_sender_details_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_sender_details_dian.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class InvoiceSenderDetailsDian(pydantic.BaseModel):
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     tax_payer_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates if the sender is a business or an individual. Can be either:\n"
-            "  \n"
+            "\n"
             "  - `Persona Jurídica`\n"
             "  - `Persona Natural`\n"
         )
     )
     regimen: typing.Optional[str] = pydantic.Field(
         description=(
             "The sender's regimen type.\n"
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_warnings_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_warnings_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_warnings_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_warnings_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoice_with_id_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoice_with_id_sat.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,30 +81,30 @@
             "*This field has been deprecated.*\n"
             "\n"
             "*The description of the payment method used for this invoice.*\n"
         )
     )
     usage: typing.Optional[str] = pydantic.Field(
         description=(
-            "The invoice's usage code, as defined by the legal entity of the country. \n"
+            "The invoice's usage code, as defined by the legal entity of the country.\n"
             "\n"
             "- 🇲🇽 Mexico [SAT catalog reference article](https://developers.belvo.com/docs/sat-catalogs#usage)\n"
         )
     )
     version: typing.Optional[str] = pydantic.Field(description=("The CFDI version of the invoice.\n"))
     place_of_issue: typing.Optional[str] = pydantic.Field(
         description=("The postcode of where the invoice was issued.\n")
     )
     invoice_details: typing.List[InvoiceDetailSat] = pydantic.Field(
         description=("A list of descriptions for each item (purchased product or service provided) in the invoice.\n")
     )
     currency: typing.Optional[str] = pydantic.Field(
         description=(
             "The currency of the invoice. For example:\n"
-            " \n"
+            "\n"
             " - 🇧🇷 BRL (Brazilian Real)\n"
             " - 🇨🇴 COP (Colombian Peso)\n"
             " - 🇲🇽 MXN (Mexican Peso)\n"
             " - 🇺🇸 USD (United States Dollar)\n"
         )
     )
     subtotal_amount: typing.Optional[float] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payments_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payments_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payments_related_documents_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payments_related_documents_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payments_related_documents_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payments_related_documents_sat.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
     invoice_identification: typing.Optional[str] = pydantic.Field(
         description=("The fiscal institution's unique ID for the related deferred invoice.\n")
     )
     currency: typing.Optional[str] = pydantic.Field(
         description=(
             "The currency of the related invoice. For example:\n"
-            "    \n"
+            "\n"
             "- 🇧🇷 BRL (Brazilian Real)\n"
             "- 🇨🇴 COP (Colombian Peso)\n"
             "- 🇲🇽 MXN (Mexican Peso)\n"
-            "  \n"
+            "\n"
             "  Please note that other currencies other than in the list above may be returned.\n"
         )
     )
     payment_method: typing.Optional[str] = pydantic.Field(description=("The payment method of the related invoice.\n"))
     partiality_number: typing.Optional[int] = pydantic.Field(description=("The payment installment number.\n"))
     previous_balance: typing.Optional[float] = pydantic.Field(description=("The invoice amount before the payment.\n"))
     amount_paid: typing.Optional[float] = pydantic.Field(description=("The amount paid in this installment.\n"))
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payments_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payments_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payroll_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payroll_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_payroll_sat.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_payroll_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_receiver_details_dian.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_receiver_details_dian.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class InvoicesReceiverDetailsDian(pydantic.BaseModel):
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     tax_payer_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates if the receiver is a business or an individual. Can be either:\n"
-            "  \n"
+            "\n"
             "  - `Persona Jurídica`\n"
             "  - `Persona Natural`\n"
         )
     )
     regimen: typing.Optional[str] = pydantic.Field(
         description=(
             "The receiver's regimen type.\n"
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_request.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/invoices_response_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/invoices_response_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_invalid_credentials.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_invalid_credentials.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_invalid_token.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_invalid_token.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_login_error.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_login_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_payment_error.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_payment_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_session_expired.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_session_expired.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/last_error_two_factor.py` & `fern_belvo-0.0.24/src/belvo/types/last_error_two_factor.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/link.py` & `fern_belvo-0.0.24/src/belvo/types/link.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/links_put_request.py` & `fern_belvo-0.0.24/src/belvo/types/links_put_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/links_request.py` & `fern_belvo-0.0.24/src/belvo/types/links_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/list_payment_links_request_ordering.py` & `fern_belvo-0.0.24/src/belvo/types/list_payment_links_request_ordering.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/list_payment_links_request_status.py` & `fern_belvo-0.0.24/src/belvo/types/list_payment_links_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/list_tax_returns_response.py` & `fern_belvo-0.0.24/src/belvo/types/list_tax_returns_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/login_error.py` & `fern_belvo-0.0.24/src/belvo/types/login_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "A unique error code (`login_error`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-login_error" target="_blank">400 login_error errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `login_error` errors, the description can be one of the following:\n"
             "\n"
             "  - `Invalid credentials provided to login to the institution`\n"
             "  - `A MFA token is required by the institution, but it's not supported yet by Belvo.`\n"
             "  - `Impossible to login, something unexpected happened while logging into the institution. Try again later.`\n"
             "  - `Login not attempted due to invalid credentials`\n"
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/needs_redirect_content.py` & `fern_belvo-0.0.24/src/belvo/types/needs_redirect_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/needs_redirect_content_pse.py` & `fern_belvo-0.0.24/src/belvo/types/needs_redirect_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/net_income_individual.py` & `fern_belvo-0.0.24/src/belvo/types/net_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_ofpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayConfirmationRequiredOfpiType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_confirmation_required: typing.Optional[DisplayConfirmationRequiredOfpi]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`, you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_pse.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayConfirmationRequiredPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_confirmation_required: typing.Optional[DisplayConfirmationRequiredContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When the value is `true`, you'll need to make a PATCH request sending through `confirm: true` to confirm the payment.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_confirmation_required_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_confirmation_required_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_credentials_required_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_credentials_required_pse.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayCredentialsRequiredPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_credentials_required: typing.Optional[DisplayCredentialsRequiredContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When the value is `true`, you'll need to make a PATCH request sending through `confirm: true` to confirm the payment.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_credentials_required_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_credentials_required_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_customer_bank_accounts_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_customer_bank_accounts_pse.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayCustomerBankAccountsPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_customer_bank_accounts: typing.Optional[DisplayCustomerBankAccountsContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When the value is `true`, you'll need to make a PATCH request sending through `confirm: true` to confirm the payment.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_needs_redirect_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_needs_redirect_pse.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayNeedsRedirectPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_needs_redirect: typing.Optional[NeedsRedirectContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When the value is `true`, you'll need to make a PATCH request sending through `confirm: true` to confirm the payment.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_needs_redirect_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_needs_redirect_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_failed.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_failed.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayPaymentFailedType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_payment_failed: typing.Optional[DisplayPaymentFailed]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`,you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_failed_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_failed_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayPaymentMethodInformationType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_payment_method_information: typing.Optional[DisplayPaymentMethodInformationContentOfpi]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`, you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_pse.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayPaymentMethodInformationPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_payment_method_information: typing.Optional[DisplayPaymentMethodInformationContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When the value is `true`, you'll need to make a PATCH request sending through `confirm: true` to confirm the payment.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_method_information_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_method_information_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_processing.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayPaymentProcessingType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_payment_processing: typing.Optional[DisplayPaymentProcessing]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`, you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_processing_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_processing_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_succeeded.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_succeeded.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepDisplayPaymentSucceededType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_payment_succeeded: typing.Optional[DisplayPaymentSucceeded]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`, you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_payment_succeeded_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_payment_succeeded_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_token_required_pse.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_token_required_pse.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
     type: typing.Optional[NextStepDisplayTokenRequiredPseType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     pse_display_token_required: typing.Optional[DisplayTokenRequiredContentPse]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. This value will return: \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed. This value will return:\n"
             "\n"
-            "  - `false` when a customer wants to pay for the very first time. This is so because you still need to input information about your customer in the following steps to process a payment successfully. \n"
-            "  - `true` when a customer wants to pay and this is not their first time. This is so because the payment intent has all the information needed about the customer to process a payment. \n"
+            "  - `false` when a customer wants to pay for the very first time. This is so because you still need to input information about your customer in the following steps to process a payment successfully.\n"
+            "  - `true` when a customer wants to pay and this is not their first time. This is so because the payment intent has all the information needed about the customer to process a payment.\n"
             "\n"
             "\n"
             "**Note:** When the value is `true`, you'll need to confirm the payment intent. You can do this by making a PATCH request sending through the parameter `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_display_token_required_pse_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_display_token_required_pse_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_needs_redirect.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_needs_redirect.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     type: typing.Optional[NextStepNeedsRedirectType] = pydantic.Field(
         description=("The type of `next_step` you need to follow.\n")
     )
     open_finance_display_needs_redirect: typing.Optional[NeedsRedirectContent]
     ready_to_confirm: typing.Optional[bool] = pydantic.Field(
         description=(
-            "Boolean that indicates whether the payment intent is ready to be confirmed. \n"
+            "Boolean that indicates whether the payment intent is ready to be confirmed.\n"
             "\n"
             "  **Note:** When set to `true`, you need to confirm the payment by making a PATCH request sending through `confirm: true`.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/next_step_needs_redirect_type.py` & `fern_belvo-0.0.24/src/belvo/types/next_step_needs_redirect_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/non_taxable_income_individual.py` & `fern_belvo-0.0.24/src/belvo/types/non_taxable_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/not_found_error_body.py` & `fern_belvo-0.0.24/src/belvo/types/not_found_error_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
             "A unique error code (`not_found`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#404-not_found" target="_blank">404 not_found errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `not_found` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `Not found`\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/owner.py` & `fern_belvo-0.0.24/src/belvo/types/owner.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/owner_document_id.py` & `fern_belvo-0.0.24/src/belvo/types/owner_document_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/owners_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/owners_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/paginated_response_link.py` & `fern_belvo-0.0.24/src/belvo/types/paginated_response_link.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/patch_body.py` & `fern_belvo-0.0.24/src/belvo/types/patch_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/patch_body_without_save_data.py` & `fern_belvo-0.0.24/src/belvo/types/patch_body_without_save_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/patch_payment_intents_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/patch_payment_intents_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/patch_payment_method_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/patch_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_institution.py` & `fern_belvo-0.0.24/src/belvo/types/payment_institution.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_ofpi_next_step.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_ofpi_next_step.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_payment_method_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_pse_last_error.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_pse_last_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intent_pse_next_step.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intent_pse_next_step.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intents_payment_method_details_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intents_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_intents_payment_method_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_intents_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_callback_urls.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_callback_urls.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_callback_urls_response.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_callback_urls_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_list_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_list_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_list_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_list_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_link_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_link_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_links_payment_method_details_body_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_links_payment_method_details_body_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_links_payment_method_details_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_links_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_details_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_information_body_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_information_body_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_information_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_information_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_information_details_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_information_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_information_ofpi.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_information_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_method_information_pse.py` & `fern_belvo-0.0.24/src/belvo/types/payment_method_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_transaction.py` & `fern_belvo-0.0.24/src/belvo/types/payment_transaction.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payment_webhook.py` & `fern_belvo-0.0.24/src/belvo/types/payment_webhook.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payments_institutions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/payments_institutions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payments_transactions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/payments_transactions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payments_way.py` & `fern_belvo-0.0.24/src/belvo/types/payments_way.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/payments_webhooks_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/payments_webhooks_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/pension_income_statement_individual.py` & `fern_belvo-0.0.24/src/belvo/types/pension_income_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/providers_pse.py` & `fern_belvo-0.0.24/src/belvo/types/providers_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/receivable_transaction_request.py` & `fern_belvo-0.0.24/src/belvo/types/receivable_transaction_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/receivables_transaction.py` & `fern_belvo-0.0.24/src/belvo/types/receivables_transaction.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/receivables_transaction_account.py` & `fern_belvo-0.0.24/src/belvo/types/receivables_transaction_account.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/receivables_transaction_number_of_installments.py` & `fern_belvo-0.0.24/src/belvo/types/receivables_transaction_number_of_installments.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/receivables_transactions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/receivables_transactions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/recevables_transaction_fees.py` & `fern_belvo-0.0.24/src/belvo/types/recevables_transaction_fees.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/recurring_expense_source_transaction.py` & `fern_belvo-0.0.24/src/belvo/types/recurring_expense_source_transaction.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/recurring_expenses.py` & `fern_belvo-0.0.24/src/belvo/types/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/recurring_expenses_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/recurring_expenses_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/recurring_expenses_request.py` & `fern_belvo-0.0.24/src/belvo/types/recurring_expenses_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/reporting_id.py` & `fern_belvo-0.0.24/src/belvo/types/reporting_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/request_timeout_error_body.py` & `fern_belvo-0.0.24/src/belvo/types/request_timeout_error_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             "A unique error code (`request_timeout`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#408-request_timeout" target="_blank">408 request_timeout errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `request_timeout` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `The request timed out, you can retry asking for less data by changing your query parameters`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/retention_breakdown.py` & `fern_belvo-0.0.24/src/belvo/types/retention_breakdown.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_balance_metrics.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_balance_metrics.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_cashflow_metrics.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_cashflow_metrics.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_credit_card_metrics.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_credit_card_metrics.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_loans_metrics.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_loans_metrics.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/risk_insights_transaction_metrics.py` & `fern_belvo-0.0.24/src/belvo/types/risk_insights_transaction_metrics.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/secret_keys.py` & `fern_belvo-0.0.24/src/belvo/types/secret_keys.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/secret_keys_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/secret_keys_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/session_expired_error.py` & `fern_belvo-0.0.24/src/belvo/types/unconfirmed_link_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class SessionExpiredError(pydantic.BaseModel):
+class UnconfirmedLinkError(pydantic.BaseModel):
     """
-    This error occurs when you try to resume a request session that has already expired. This is usually because the user took too long to provide their authentication token.
+    This error occurs when you try to access a link that was paused previously (and as such is not active now).
+    A Link's status is set to `unconfirmed_link` when your user has not completed the Link creation process successfully (for example, they might not provide a valid MFA token).
     """
 
     code: typing.Optional[str] = pydantic.Field(
         description=(
-            "A unique error code (`session_expired`) that allows you to classify and handle the error programmatically.\n"
+            "A unique error code (`unconfirmed_link`) that allows you to classify and handle the error programmatically.\n"
             "\n"
-            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-session_expired" target="_blank">400 session_expired errors</a>.\n'
+            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-unconfirmed_link" target="_blank">400 unconfirmed_link errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
-            "For `session_expired` errors, the description is:\n"
-            "  \n"
-            "  - `The session you are trying to resume has expired, please start again from register/retrieve endpoint`.\n"
+            "For `unconfirmed_link` errors, the description is:\n"
+            "\n"
+            "  - `The link creation has not been completed yet`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
     )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/standard_request.py` & `fern_belvo-0.0.24/src/belvo/types/standard_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_assessment_business.py` & `fern_belvo-0.0.24/src/belvo/types/tax_assessment_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_assessment_individual.py` & `fern_belvo-0.0.24/src/belvo/types/tax_assessment_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_compliance_status.py` & `fern_belvo-0.0.24/src/belvo/types/tax_compliance_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_compliance_status_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/tax_compliance_status_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_compliance_status_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_compliance_status_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_declaration_business.py` & `fern_belvo-0.0.24/src/belvo/types/tax_declaration_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_declaration_business_paginated.py` & `fern_belvo-0.0.24/src/belvo/types/tax_declaration_business_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_declaration_individual.py` & `fern_belvo-0.0.24/src/belvo/types/tax_declaration_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_declaration_individual_paginated.py` & `fern_belvo-0.0.24/src/belvo/types/tax_declaration_individual_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_declarations_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_declarations_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_payer_information_business.py` & `fern_belvo-0.0.24/src/belvo/types/tax_payer_information_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_payer_information_individual.py` & `fern_belvo-0.0.24/src/belvo/types/tax_payer_information_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_retentions.py` & `fern_belvo-0.0.24/src/belvo/types/tax_retentions.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_retentions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/tax_retentions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_retentions_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_retentions_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_returns_monthly_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_returns_monthly_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_returns_yearly_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_returns_yearly_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_address_between_street_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_address_between_street_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_address_between_street_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_address_between_street_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_address_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_address_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_address_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_address_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_economic_activity_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_economic_activity_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_economic_activity_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_economic_activity_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_obligations_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_obligations_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_obligations_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_obligations_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_regimens_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_regimens_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_regimens_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_regimens_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_request.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_tax_payer_information_dian.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_tax_payer_information_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/tax_status_tax_payer_information_sat.py` & `fern_belvo-0.0.24/src/belvo/types/tax_status_tax_payer_information_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/token_required_response.py` & `fern_belvo-0.0.24/src/belvo/types/token_required_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
             "A unique error code (`token_required`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#428-token_required" target="_blank">428 token_required errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `token_required` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `A MFA token is required by the institution to login`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/token_required_response_token_generation_data.py` & `fern_belvo-0.0.24/src/belvo/types/token_required_response_token_generation_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/too_many_sessions_error.py` & `fern_belvo-0.0.24/src/belvo/types/too_many_sessions_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
             "A unique error code (`too_many_sessions`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-too_many_sessions" target="_blank">400 too_many_sessions errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `too_many_sessions` errors, the description is:\n"
-            "  \n"
+            "\n"
             "  - `Impossible to login, a session is already opened with the institution for these credentials`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/transaction.py` & `fern_belvo-0.0.24/src/belvo/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/transaction_bank_account_body_pse.py` & `fern_belvo-0.0.24/src/belvo/types/transaction_bank_account_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/transaction_credit_card_data.py` & `fern_belvo-0.0.24/src/belvo/types/transaction_credit_card_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/transaction_merchant_data.py` & `fern_belvo-0.0.24/src/belvo/types/transaction_merchant_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/transactions_paginated_response.py` & `fern_belvo-0.0.24/src/belvo/types/transactions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/transactions_request.py` & `fern_belvo-0.0.24/src/belvo/types/transactions_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.23/src/belvo/types/unauthorized_error_body.py` & `fern_belvo-0.0.24/src/belvo/types/unauthorized_error_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "A unique error code (`authentication_failed`) that allows you to classify and handle the error programmatically.\n"
             "\n"
             'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#401-authentication_failed" target="_blank">401 authentication_failed errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `authentication_failed` errors, the description is:\n"
             "\n"
             "  - `Invalid Secret Keys`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/unconfirmed_link_error.py` & `fern_belvo-0.0.24/src/belvo/types/unexpected_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class UnconfirmedLinkError(pydantic.BaseModel):
+class UnexpectedError(pydantic.BaseModel):
     """
-    This error occurs when you try to access a link that was paused previously (and as such is not active now).
-    A Link's status is set to `unconfirmed_link` when your user has not completed the Link creation process successfully (for example, they might not provide a valid MFA token).
+    This error occurs when we (Belvo) have encountered an internal system error (sorry about that) or due to an unsupported response from the institution.
     """
 
     code: typing.Optional[str] = pydantic.Field(
         description=(
-            "A unique error code (`unconfirmed_link`) that allows you to classify and handle the error programmatically.\n"
+            "A unique error code (`unexpected_error`) that allows you to classify and handle the error programmatically.\n"
             "\n"
-            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-unconfirmed_link" target="_blank">400 unconfirmed_link errors</a>.\n'
+            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#500-unexpected_error" target="_blank">500 unexpected_error errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
-            "For `unconfirmed_link` errors, the description is:\n"
-            "  \n"
-            "  - `The link creation has not been completed yet`.\n"
+            "For `unexpected_error` errors, the description is:\n"
+            "\n"
+            "  - `Belvo is unable to process the request due to an internal system issue or to an unsupported response from an institution`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
     )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/unexpected_error.py` & `fern_belvo-0.0.24/src/belvo/types/unsupported_operation_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class UnexpectedError(pydantic.BaseModel):
+class UnsupportedOperationError(pydantic.BaseModel):
     """
-    This error occurs when we (Belvo) have encountered an internal system error (sorry about that) or due to an unsupported response from the institution.
+    This error occurs when you try to access some data operation that Belvo does not support for an institution. For example, trying to access the Balances resource for fiscal institutions.
     """
 
     code: typing.Optional[str] = pydantic.Field(
         description=(
-            "A unique error code (`unexpected_error`) that allows you to classify and handle the error programmatically.\n"
+            "A unique error code (`unsupported_operation`) that allows you to classify and handle the error programmatically.\n"
             "\n"
-            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#500-unexpected_error" target="_blank">500 unexpected_error errors</a>.\n'
+            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-unsupported_operation" target="_blank">400 unsupported_operation errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
-            "For `unexpected_error` errors, the description is:\n"
-            "  \n"
-            "  - `Belvo is unable to process the request due to an internal system issue or to an unsupported response from an institution`.\n"
+            "For `unsupported_operation` errors, the description is:\n"
+            "\n"
+            "  - `The resource you are trying to access is not supported by this institution`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
     )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/unsupported_operation_error.py` & `fern_belvo-0.0.24/src/belvo/types/invalid_link_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class UnsupportedOperationError(pydantic.BaseModel):
+class InvalidLinkError(pydantic.BaseModel):
     """
-    This error occurs when you try to access some data operation that Belvo does not support for an institution. For example, trying to access the Balances resource for fiscal institutions.
+    This error occurs when you try to access an account but the user credentials are no longer valid, prompting an error from the institution.
     """
 
     code: typing.Optional[str] = pydantic.Field(
         description=(
-            "A unique error code (`unsupported_operation`) that allows you to classify and handle the error programmatically.\n"
+            "A unique error code (`invalid_link`) that allows you to classify and handle the error programmatically.\n"
             "\n"
-            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-unsupported_operation" target="_blank">400 unsupported_operation errors</a>.\n'
+            'ℹ️ Check our DevPortal for more information on how to handle <a href="https://developers.belvo.com/docs/belvo-api-errors#400-invalid_link" target="_blank">400 invalid_link errors</a>.\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
-            "For `unsupported_operation` errors, the description is:\n"
-            "  \n"
-            "  - `The resource you are trying to access is not supported by this institution`.\n"
+            "For `invalid_link` errors, the description is:\n"
+            "\n"
+            "  - `The link has been invalidated. You may need to update link credentials`.\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
         description=(
             "A 32-character unique ID of the request (matching a regex pattern of: `[a-f0-9]{32}`). Provide this ID when contacting the Belvo support team to accelerate investigations.\n"
         )
     )
```

### Comparing `fern_belvo-0.0.23/src/belvo/types/validation_error.py` & `fern_belvo-0.0.24/src/belvo/types/validation_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
             '  - <a href="https://developers.belvo.com/docs/belvo-api-errors#400-null" target="_blank">400 null errors</a>\n'
             '  - <a href="https://developers.belvo.com/docs/belvo-api-errors#400-does_not_exist" target="_blank">400 does_not_exist errors</a>\n'
             '  - <a href="https://developers.belvo.com/docs/belvo-api-errors#400-required" target="_blank">400 required errors</a>\n'
         )
     )
     message: typing.Optional[str] = pydantic.Field(
         description=(
-            "A short description of the error. \n"
+            "A short description of the error.\n"
             "\n"
             "For `session_expired` errors, the description can be (among others):\n"
-            "  \n"
+            "\n"
             "  - `This field is required.`\n"
             "  - `Object with name=narnia does not exist.`\n"
             "  - `This field may not be null.`\n"
             "  - `This field may not be blank.`\n"
         )
     )
     request_id: typing.Optional[str] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.23/PKG-INFO` & `fern_belvo-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-belvo
-Version: 0.0.23
+Version: 0.0.24
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

