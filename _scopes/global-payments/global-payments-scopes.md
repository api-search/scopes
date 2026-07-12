---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Global Payments Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Global Payments publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Global Payments API on a user''s behalf.


  Tokens are issued from https://apis.globalpay.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Global Payments
provider_slug: global-payments
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.globalpay.com/oauth2/token
  name: oauth2
  source: openapi/global-payments-unified-payments-api-openapi.yml
scope_count: 4
scope_names:
- payment-methods:read
- payment-methods:write
- transactions:read
- transactions:write
scopes:
- description: Read payment methods
  flows:
  - clientCredentials
  scope: payment-methods:read
- description: Store payment methods
  flows:
  - clientCredentials
  scope: payment-methods:write
- description: Read transactions
  flows:
  - clientCredentials
  scope: transactions:read
- description: Create transactions
  flows:
  - clientCredentials
  scope: transactions:write
slug: global-payments-scopes
source_filename: global-payments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/global-payments-unified-payments-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/global-payments-unified-payments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.globalpay.com/oauth2/token\nscopes:\n- scope: payment-methods:read\n  description: Read payment methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n- scope: payment-methods:write\n  description: Store payment methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n- scope: transactions:read\n  description: Read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n- scope: transactions:write\n  description: Create transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-payments/refs/heads/main/scopes/global-payments-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- eCommerce
- Payment Processing
- Payment Technology
- Payments
- POS
- Fortune 1000
token_urls:
- https://apis.globalpay.com/oauth2/token
---
