---
authorization_urls: []
description: ''
docs: https://developer.alloy.com/public/docs/authentication-guide
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Alloy Scopes
name_suffix: OAuth Scopes
note: Alloy's API uses OAuth 2.0 client_credentials (API token/secret exchanged for a one-hour bearer token) or Basic HTTP auth, and does not use or document OAuth scopes (https://developer.alloy.com/public/docs/authentication-guide).
overview: 'Alloy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/bearer.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alloy
provider_slug: alloy
schemes:
- description: OAuth2 using a workflow token and secret to generate a bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/bearer
  name: oauth2
  source: openapi/alloy-identity-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: alloy-scopes
source_filename: alloy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-identity-api-openapi.yml\ndocs: https://developer.alloy.com/public/docs/authentication-guide\nnote: Alloy's API uses OAuth 2.0 client_credentials (API token/secret exchanged for a\n  one-hour bearer token) or Basic HTTP auth, and does not use or document OAuth scopes\n  (https://developer.alloy.com/public/docs/authentication-guide).\nschemes:\n- name: oauth2\n  source: openapi/alloy-identity-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/bearer\n  description: OAuth2 using a workflow token and secret to generate a bearer token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/scopes/alloy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Identity Verification
- KYC
- KYB
- Fraud Prevention
- Compliance
- Onboarding
- Transaction Monitoring
- Risk Decisioning
- AML
- Fintech
token_urls:
- /oauth/bearer
---
