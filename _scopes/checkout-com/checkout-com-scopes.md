---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Checkout Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Checkout.com publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Checkout.com API on a user''s behalf.


  Tokens are issued from https://access.checkout.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Checkout.com
provider_slug: checkout-com
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://access.checkout.com/connect/token
  name: OAuth2
  source: openapi/checkout-com-openapi.yml
scope_count: 2
scope_names:
- gateway
- vault
scopes:
- description: Access to gateway resources
  flows:
  - clientCredentials
  scope: gateway
- description: Access to vault resources
  flows:
  - clientCredentials
  scope: vault
slug: checkout-com-scopes
source_filename: checkout-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkout-com-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/checkout-com-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://access.checkout.com/connect/token\n  description: OAuth 2.0 client credentials flow\nscopes:\n- scope: gateway\n  description: Access to gateway resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/checkout-com-openapi.yml\n- scope: vault\n  description: Access to vault resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/checkout-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/scopes/checkout-com-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Fintech
- Payments
- Cards
- Acquiring
- Cross-Border
token_urls:
- https://access.checkout.com/connect/token
---
