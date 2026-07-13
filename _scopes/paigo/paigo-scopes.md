---
api_specs:
- filename: public_api.html
  format: yaml
  label: Paigo API
  slug: paigo-api
  spec_type: OpenAPI
  url: https://paigo-public-information.s3.us-east-2.amazonaws.com/public_api.html
authorization_urls: []
description: ''
docs: https://docs.paigo.tech/overview/getting-started-with-paigo
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Paigo Scopes
name_suffix: OAuth Scopes
note: Paigo uses an OAuth 2.0 client_credentials flow (token from https://auth.paigo.tech/oauth/token with client ID/secret from Settings > API) and does not document or use OAuth scopes (https://docs.paigo.tech/overview/getting-started-with-paigo).
overview: 'Paigo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.paigo.tech/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paigo
provider_slug: paigo
schemes:
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-paigo-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paigo-scopes
source_filename: paigo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paigo-paigo-api-openapi.yml\ndocs: https://docs.paigo.tech/overview/getting-started-with-paigo\nnote: Paigo uses an OAuth 2.0 client_credentials flow (token from https://auth.paigo.tech/oauth/token with client ID/secret from Settings > API) and does not document or use OAuth scopes (https://docs.paigo.tech/overview/getting-started-with-paigo).\nschemes:\n- name: bearer\n  source: openapi/paigo-paigo-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/scopes/paigo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Billing
- Usage-Based Billing
- Metering
- Invoicing
- Pricing
- SaaS
- Subscriptions
- Developer Tools
- FinOps
token_urls:
- https://auth.paigo.tech/oauth/token
---
