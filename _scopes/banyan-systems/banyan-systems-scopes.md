---
api_specs:
- filename: banyan-systems-authentication-api-openapi.yml
  format: yaml
  label: Banyan Systems Authentication API
  slug: banyan-systems-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-authentication-api-openapi.yml
- filename: banyan-systems-card-linked-offer-api-openapi.yml
  format: yaml
  label: Banyan Systems Card Linked Offer API
  slug: banyan-systems-card-linked-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-card-linked-offer-api-openapi.yml
- filename: banyan-systems-consent-api-openapi.yml
  format: yaml
  label: Banyan Systems Consent API
  slug: banyan-systems-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-consent-api-openapi.yml
- filename: banyan-systems-enriched-data-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data API
  slug: banyan-systems-enriched-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-api-openapi.yml
- filename: banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data - Merchant Service Provider API
  slug: banyan-systems-enriched-data-merchant-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
- filename: banyan-systems-history-api-openapi.yml
  format: yaml
  label: Banyan Systems History API
  slug: banyan-systems-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-history-api-openapi.yml
- filename: banyan-systems-receipt-api-openapi.yml
  format: yaml
  label: Banyan Systems Receipt API
  slug: banyan-systems-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-receipt-api-openapi.yml
- filename: banyan-systems-tag-counter-api-openapi.yml
  format: yaml
  label: Banyan Systems Tag Counter API
  slug: banyan-systems-tag-counter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-tag-counter-api-openapi.yml
- filename: banyan-systems-transaction-api-openapi.yml
  format: yaml
  label: Banyan Systems Transaction API
  slug: banyan-systems-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-transaction-api-openapi.yml
- filename: banyan-systems-webhook-api-openapi.yml
  format: yaml
  label: Banyan Systems Webhook API
  slug: banyan-systems-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-webhook-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Banyan Systems Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Banyan Systems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Banyan Systems
provider_slug: banyan-systems
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: bearerToken
  source: openapi/banyan-systems-rest-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: bearerToken
  source: openapi/banyan-systems-sensitive-data-vault-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: banyan-systems-scopes
source_filename: banyan-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/banyan-systems-rest-api-openapi.yml, openapi/banyan-systems-sensitive-data-vault-openapi.yml\nschemes:\n- name: bearerToken\n  source: openapi/banyan-systems-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n- name: bearerToken\n  source: openapi/banyan-systems-sensitive-data-vault-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/scopes/banyan-systems-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Receipt Data
- Transaction Enrichment
- Item-Level Data
- Card-Linked Offers
- Fintech
- Payments
- Data Collaboration
- Webhook
- Data Enrichment
token_bound: false
token_urls:
- /oauth/token
---
