---
api_specs:
- filename: rtr-inbound-participant-payment-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Participant Payment API
  slug: rtr-inbound-participant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-participant-payment-api-openapi.yml
- filename: rtr-inbound-csp-heartbeat-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Exchange Heartbeat API
  slug: rtr-inbound-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
- filename: rtr-interest-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Interest Report API
  slug: rtr-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-interest-report-api-openapi.yml
- filename: rtr-balance-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Payment Capacity Balance Report API
  slug: rtr-balance-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-balance-report-api-openapi.yml
- filename: fif-extracts-api-openapi.yml
  format: yaml
  label: FIF Extracts API
  slug: fif-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-extracts-api-openapi.yml
- filename: fif-branch-api-openapi.yml
  format: yaml
  label: FIF Branch API
  slug: fif-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-branch-api-openapi.yml
- filename: ccin-extracts-api-openapi.yml
  format: yaml
  label: CCIN Extracts API
  slug: ccin-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-extracts-api-openapi.yml
- filename: ccin-lookup-api-openapi.yml
  format: yaml
  label: CCIN Lookup API
  slug: ccin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-lookup-api-openapi.yml
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
- Financial Services
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
