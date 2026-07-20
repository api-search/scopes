---
api_specs:
- filename: balad-corp-gateway-openapi.yml
  format: yaml
  label: Balad Gateway API
  slug: balad-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-gateway-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.balad.tech/authorization-1459814m0.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Balad Corp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BALAD CORP uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BALAD CORP
provider_slug: balad-corp
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  source: openapi/balad-corp-gateway-openapi.yml
  tokenUrl: /identity/v1/token
scope_count: 0
scope_names: []
scopes: []
slug: balad-corp-scopes
source_filename: balad-corp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.balad.tech/authorization-1459814m0.md\ndocs: https://developers.balad.tech/authorization-1459814m0.md\nschemes:\n  - name: OAuth2ClientCredentials\n    flow: clientCredentials\n    tokenUrl: /identity/v1/token\n    source: openapi/balad-corp-gateway-openapi.yml\n# Balad documents that access tokens are \"scoped to specific APIs\" and returns a `scope`\n# claim on the token response, but does NOT publish an enumerated scope/permission reference.\n# The product-area scope groups below are the granularity Balad names in its docs; individual\n# scope string values are not published and are therefore NOT invented here.\nscope_groups:\n  - name: remittances\n    description: Balad Link money-transfer / payout APIs (create, cancel, status, reconciliation).\n  - name: collections\n    description: Collection / invoice APIs (referenced in docs; not enabled for all partners).\n  - name: bills\n    description: Bill\
  \ payment APIs (billers, providers, bill payments).\n  - name: vouchers\n    description: Voucher APIs (referenced in docs).\nscopes: []\nnotes: Enumerated scope values are not published by Balad; only product-area scoping is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/scopes/balad-corp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Payments
- Remittances
- Cross-Border Payments
- Fintech
- Egypt
- Payouts
- Money Transfer
- Banking
- API
token_urls: []
---
