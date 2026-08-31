---
api_specs:
- filename: payments-canada-application-level-heartbeat-api-openapi.yml
  format: yaml
  label: Payments Canada application level heartbeat API
  slug: payments-canada-application-level-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-application-level-heartbeat-api-openapi.yml
- filename: payments-canada-ccin-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Ccin Extract Resource API
  slug: payments-canada-ccin-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-ccin-extract-resource-api-openapi.yml
- filename: payments-canada-fif-branches-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Fif Branches Resource API
  slug: payments-canada-fif-branches-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-fif-branches-resource-api-openapi.yml
- filename: payments-canada-fif-extracts-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Fif Extracts Resource API
  slug: payments-canada-fif-extracts-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-fif-extracts-resource-api-openapi.yml
- filename: payments-canada-interest-report-api-openapi.yml
  format: yaml
  label: Payments Canada Interest Report API
  slug: payments-canada-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-interest-report-api-openapi.yml
- filename: payments-canada-master-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Master Extract Resource API
  slug: payments-canada-master-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-master-extract-resource-api-openapi.yml
- filename: payments-canada-report-api-openapi.yml
  format: yaml
  label: Payments Canada Report API
  slug: payments-canada-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-report-api-openapi.yml
- filename: payments-canada-single-credit-transfer-api-openapi.yml
  format: yaml
  label: Payments Canada single credit transfer API
  slug: payments-canada-single-credit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-single-credit-transfer-api-openapi.yml
- filename: payments-canada-single-credit-transfer-status-enquiry-api-openapi.yml
  format: yaml
  label: Payments Canada single credit transfer status enquiry API
  slug: payments-canada-single-credit-transfer-status-enquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-single-credit-transfer-status-enquiry-api-openapi.yml
- filename: payments-canada-update-extract-resource-api-openapi.yml
  format: yaml
  label: Payments Canada Update Extract Resource API
  slug: payments-canada-update-extract-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/payments-canada-update-extract-resource-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Payments Canada Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Payments Canada publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Payments Canada API on a user''s behalf.


  Tokens are issued from https://api.payments.ca/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Payments Canada
provider_slug: payments-canada
schemes:
- description: This API uses OAuth 2 with the implicit grant flow. (The access token expires in 5 minutes)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.payments.ca/accesstoken
  name: oAuth
  source: openapi/rtr-balance-report-api-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow. (The access token expires in 5 minutes)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.payments.ca/accesstoken
  name: oAuth
  source: openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow. (The access token expires in 5 minutes)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.payments.ca/accesstoken
  name: oAuth
  source: openapi/rtr-inbound-participant-payment-api-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow. (The access token expires in 5 minutes)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.payments.ca/accesstoken
  name: oAuth
  source: openapi/rtr-interest-report-api-openapi.yml
scope_count: 1
scope_names:
- client_credentials
scopes:
- description: Required to get credentials for the API call
  flows:
  - clientCredentials
  scope: client_credentials
slug: payments-canada-scopes
source_filename: payments-canada-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/rtr-balance-report-api-openapi.yml, openapi/rtr-inbound-csp-heartbeat-api-openapi.yml,\n  openapi/rtr-inbound-participant-payment-api-openapi.yml, openapi/rtr-interest-report-api-openapi.yml\nschemes:\n- name: oAuth\n  source: openapi/rtr-balance-report-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.payments.ca/accesstoken\n  description: This API uses OAuth 2 with the implicit grant flow. (The access token expires\n    in 5 minutes)\n- name: oAuth\n  source: openapi/rtr-inbound-csp-heartbeat-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.payments.ca/accesstoken\n  description: This API uses OAuth 2 with the implicit grant flow. (The access token expires\n    in 5 minutes)\n- name: oAuth\n  source: openapi/rtr-inbound-participant-payment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.payments.ca/accesstoken\n  description:\
  \ This API uses OAuth 2 with the implicit grant flow. (The access token expires\n    in 5 minutes)\n- name: oAuth\n  source: openapi/rtr-interest-report-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.payments.ca/accesstoken\n  description: This API uses OAuth 2 with the implicit grant flow. (The access token expires\n    in 5 minutes)\nscopes:\n- scope: client_credentials\n  description: Required to get credentials for the API call\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/rtr-balance-report-api-openapi.yml\n  - openapi/rtr-inbound-csp-heartbeat-api-openapi.yml\n  - openapi/rtr-inbound-participant-payment-api-openapi.yml\n  - openapi/rtr-interest-report-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/scopes/payments-canada-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Financial-Services
- Payments
- Canada
- Payment Infrastructure
- Clearing and Settlement
- Real-Time Rail
- ISO 20022
- Lynx
- Crown Corporation
- Faster Payments
token_urls:
- https://api.payments.ca/accesstoken
---
