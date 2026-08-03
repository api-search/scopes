---
api_specs:
- filename: amex-gbt-user-sync-api-openapi.json
  format: json
  label: Egencia User Sync API
  slug: egencia-user-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-user-sync-api-openapi.json
- filename: amex-gbt-sso-context-api-openapi.json
  format: json
  label: Egencia Context SSO API
  slug: egencia-context-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-sso-context-api-openapi.json
- filename: amex-gbt-company-info-api-openapi.json
  format: json
  label: Egencia Company Details API
  slug: egencia-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-info-api-openapi.json
- filename: amex-gbt-company-cdf-api-openapi.json
  format: json
  label: Egencia Company CDF API
  slug: egencia-company-cdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-cdf-api-openapi.json
- filename: amex-gbt-validation-spi-openapi.json
  format: json
  label: Egencia Validation SPI
  slug: egencia-validation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-validation-spi-openapi.json
- filename: amex-gbt-expense-spi-openapi.json
  format: json
  label: Egencia Expense SPI
  slug: egencia-expense-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-expense-spi-openapi.json
- filename: amex-gbt-booking-api-openapi.json
  format: json
  label: Egencia Get Booking API
  slug: egencia-get-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-booking-api-openapi.json
- filename: amex-gbt-cancellation-deletion-api-openapi.json
  format: json
  label: Egencia Expense Cancellation and Deletion API
  slug: egencia-cancellation-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-cancellation-deletion-api-openapi.json
- filename: amex-gbt-approval-workflow-api-openapi.json
  format: json
  label: Egencia Approval Workflow API
  slug: egencia-approval-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-workflow-api-openapi.json
- filename: amex-gbt-approval-customisation-spi-openapi.json
  format: json
  label: Egencia Approval Customisation SPI
  slug: egencia-approval-customisation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-customisation-spi-openapi.json
- filename: amex-gbt-receipt-api-openapi.json
  format: json
  label: Egencia Receipt API
  slug: egencia-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-receipt-api-openapi.json
- filename: amex-gbt-duty-of-care-api-openapi.json
  format: json
  label: Egencia Duty of Care API
  slug: egencia-duty-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-duty-of-care-api-openapi.json
- filename: amex-gbt-reporting-api-openapi.json
  format: json
  label: Egencia Reporting API (BI Transactions)
  slug: egencia-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-reporting-api-openapi.json
- filename: amex-gbt-service-bi-openapi.json
  format: json
  label: American Express Global Business Travel BI API
  slug: amex-gbt-service-bi-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-bi-openapi.json
- filename: amex-gbt-service-company-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Company)
  slug: amex-gbt-service-company-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-company-openapi.json
- filename: amex-gbt-service-dutyofcare-openapi.json
  format: json
  label: American Express Global Business Travel Duty Of Care API
  slug: amex-gbt-service-dutyofcare-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-dutyofcare-openapi.json
- filename: amex-gbt-service-openconnect-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Openconnect)
  slug: amex-gbt-service-openconnect-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-openconnect-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Amex Gbt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'American Express Global Business Travel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://apis.egencia.com/auth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: American Express Global Business Travel
provider_slug: amex-gbt
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-approval-workflow-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-booking-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-cancellation-deletion-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-company-cdf-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: oAuth2
  source: openapi/amex-gbt-company-info-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-duty-of-care-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-receipt-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-reporting-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-service-bi-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: oAuth2
  source: openapi/amex-gbt-service-company-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-service-dutyofcare-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-service-openconnect-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.egencia.com/auth/v1/token
  name: OAuth2
  source: openapi/amex-gbt-user-sync-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: amex-gbt-scopes
source_filename: amex-gbt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/amex-gbt-approval-workflow-api-openapi.json, openapi/amex-gbt-booking-api-openapi.json,\n  openapi/amex-gbt-cancellation-deletion-api-openapi.json, openapi/amex-gbt-company-cdf-api-openapi.json,\n  openapi/amex-gbt-company-info-api-openapi.json, openapi/amex-gbt-duty-of-care-api-openapi.json,\n  openapi/amex-gbt-receipt-api-openapi.json, openapi/amex-gbt-reporting-api-openapi.json, openapi/amex-gbt-service-bi-openapi.json,\n  openapi/amex-gbt-service-company-openapi.json, openapi/amex-gbt-service-dutyofcare-openapi.json,\n  openapi/amex-gbt-service-openconnect-openapi.json, openapi/amex-gbt-user-sync-api-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/amex-gbt-approval-workflow-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-booking-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-cancellation-deletion-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-company-cdf-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: oAuth2\n  source: openapi/amex-gbt-company-info-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-duty-of-care-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-receipt-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-reporting-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-service-bi-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: oAuth2\n  source: openapi/amex-gbt-service-company-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-service-dutyofcare-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-service-openconnect-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\n- name: OAuth2\n  source: openapi/amex-gbt-user-sync-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.egencia.com/auth/v1/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/scopes/amex-gbt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Travel
- United States
- Corporate Travel
- Travel Management
- Business Travel
- Distribution
- Booking
- Aviation
- Hotels
- Rail
- Car Rental
- Expense
- Duty of Care
- Reporting
token_urls:
- https://apis.egencia.com/auth/v1/token
---
