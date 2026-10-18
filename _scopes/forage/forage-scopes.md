---
api_specs:
- filename: forage-payments-api-openapi.yml
  format: yaml
  label: Forage EBT SNAP Payments API
  slug: forage-ebt-snap-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payments-api-openapi.yml
- filename: forage-bearer-tokens-api-openapi.yml
  format: yaml
  label: Forage Bearer Tokens API
  slug: forage-bearer-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-bearer-tokens-api-openapi.yml
- filename: forage-card-details-api-openapi.yml
  format: yaml
  label: Forage Card Details API
  slug: forage-card-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-card-details-api-openapi.yml
- filename: forage-custom-sessions-api-openapi.yml
  format: yaml
  label: Forage Custom Sessions API
  slug: forage-custom-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-custom-sessions-api-openapi.yml
- filename: forage-deferred-capture-api-openapi.yml
  format: yaml
  label: Forage Deferred Capture API
  slug: forage-deferred-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-deferred-capture-api-openapi.yml
- filename: forage-fully-hosted-sessions-api-openapi.yml
  format: yaml
  label: Forage Fully Hosted Sessions API
  slug: forage-fully-hosted-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-fully-hosted-sessions-api-openapi.yml
- filename: forage-order-payments-api-openapi.yml
  format: yaml
  label: Forage Order Payments API
  slug: forage-order-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-payments-api-openapi.yml
- filename: forage-order-refunds-api-openapi.yml
  format: yaml
  label: Forage Order Refunds API
  slug: forage-order-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-refunds-api-openapi.yml
- filename: forage-orders-api-openapi.yml
  format: yaml
  label: Forage Orders API
  slug: forage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-orders-api-openapi.yml
- filename: forage-payment-methods-api-openapi.yml
  format: yaml
  label: Forage Payment Methods API
  slug: forage-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-methods-api-openapi.yml
- filename: forage-payment-refunds-api-openapi.yml
  format: yaml
  label: Forage Payment Refunds API
  slug: forage-payment-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-refunds-api-openapi.yml
- filename: forage-reports-api-openapi.yml
  format: yaml
  label: Forage Reports API
  slug: forage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-reports-api-openapi.yml
- filename: forage-sandbox-testing-api-openapi.yml
  format: yaml
  label: Forage Sandbox Testing API
  slug: forage-sandbox-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-sandbox-testing-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Forage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Forage publishes 6 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Forage API on a user''s behalf.


  Tokens are issued from /o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Forage
provider_slug: forage
schemes:
- description: Pass the access token in the 'Authorization' header with the format "Bearer ${token}", i.e. the word "Bearer" and your access token from the /o/token/ API, separated by whitespace.
  flows:
  - flow: password
    tokenUrl: /o/token/
  - flow: clientCredentials
    tokenUrl: /o/token/
  name: OAuth2
  source: openapi/forage-payments-api-openapi.yml
scope_count: 6
scope_names:
- disbursement
- hosted_checkout
- internal
- pin-protected
- pinpad_only
- reporting
scopes:
- description: Scope for tokens which can disburse money to merchants.
  flows:
  - clientCredentials
  scope: disbursement
- description: Scope for tokens used by merchant applications which allow Forage to manage split tender processing (i.e. EBT + Credit/Debit).
  flows:
  - password
  scope: hosted_checkout
- description: Scope for tokens used by Forage internal applications.
  flows:
  - clientCredentials
  scope: internal
- description: Scope for tokens which can access secure storage.
  flows:
  - clientCredentials
  scope: pin-protected
- description: Scope for tokens used by merchant applications which manage their own split tender (i.e. Forage Checkout is used only for EBT processing).
  flows:
  - password
  scope: pinpad_only
- description: ''
  flows: []
  scope: reporting
slug: forage-scopes
source_filename: forage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/forage-payments-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/forage-payments-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /o/token/\n  - flow: clientCredentials\n    tokenUrl: /o/token/\n  description: Pass the access token in the 'Authorization' header with the format \"Bearer ${token}\",\n    i.e. the word \"Bearer\" and your access token from the /o/token/ API, separated by whitespace.\nscopes:\n- scope: disbursement\n  description: Scope for tokens which can disburse money to merchants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n- scope: hosted_checkout\n  description: Scope for tokens used by merchant applications which allow Forage to manage split\n    tender processing (i.e. EBT + Credit/Debit).\n  flows:\n  - password\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n- scope: internal\n  description: Scope for tokens used\
  \ by Forage internal applications.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n- scope: pin-protected\n  description: Scope for tokens which can access secure storage.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n- scope: pinpad_only\n  description: Scope for tokens used by merchant applications which manage their own split tender\n    (i.e. Forage Checkout is used only for EBT processing).\n  flows:\n  - password\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n- scope: reporting\n  sources:\n  - openapi/forage-payments-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/scopes/forage-scopes.yml
summary_line: 6 scopes · password/clientCredentials
tags:
- Company
- Payments
- EBT
- SNAP
- EBT Cash
- HSA/FSA
- Fintech
- Government Benefits
- Grocery
- Checkout
- Financial Services
token_bound: false
token_urls:
- /o/token/
---
