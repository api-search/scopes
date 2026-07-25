---
api_specs:
- filename: scotiabank-account-validation-api-openapi.yml
  format: yaml
  label: Scotiabank Account Validation API
  slug: scotiabank-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-account-validation-api-openapi.yml
- filename: scotiabank-accounts-api-openapi.yml
  format: yaml
  label: Scotiabank Accounts API
  slug: scotiabank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-accounts-api-openapi.yml
- filename: scotiabank-eft-payments-api-openapi.yml
  format: yaml
  label: Scotiabank EFT Payments API
  slug: scotiabank-eft-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-eft-payments-api-openapi.yml
- filename: scotiabank-payment-tracking-api-openapi.yml
  format: yaml
  label: Scotiabank Payment Tracking API
  slug: scotiabank-payment-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-payment-tracking-api-openapi.yml
- filename: scotiabank-real-time-payments-api-openapi.yml
  format: yaml
  label: Scotiabank Real-Time Payments API
  slug: scotiabank-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-real-time-payments-api-openapi.yml
- filename: scotiabank-request-for-payment-api-openapi.yml
  format: yaml
  label: Scotiabank Request for Payment API
  slug: scotiabank-request-for-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-request-for-payment-api-openapi.yml
- filename: scotiabank-wire-payments-api-openapi.yml
  format: yaml
  label: Scotiabank Wire Payments API
  slug: scotiabank-wire-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-wire-payments-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Scotiabank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Scotiabank publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Scotiabank API on a user''s behalf.


  Tokens are issued from https://developer.api.scotiabank.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scotiabank
provider_slug: scotiabank
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.scotiabank.com/auth/token
  name: OAuth2
  source: openapi/scotiabank-tranxact-openapi.yml
scope_count: 3
scope_names:
- accounts:read
- payments:read
- payments:write
scopes:
- description: Read account information
  flows:
  - clientCredentials
  scope: accounts:read
- description: Read payment status
  flows:
  - clientCredentials
  scope: payments:read
- description: Initiate payments
  flows:
  - clientCredentials
  scope: payments:write
slug: scotiabank-scopes
source_filename: scotiabank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scotiabank-tranxact-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/scotiabank-tranxact-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.scotiabank.com/auth/token\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/scotiabank-tranxact-openapi.yml\n- scope: payments:read\n  description: Read payment status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/scotiabank-tranxact-openapi.yml\n- scope: payments:write\n  description: Initiate payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/scotiabank-tranxact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/scopes/scotiabank-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Banking
- Finance
- Payments
- Canada
- Open Banking
token_urls:
- https://developer.api.scotiabank.com/auth/token
---
