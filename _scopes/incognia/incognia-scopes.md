---
api_specs:
- filename: incognia-openapi-original.yml
  format: yaml
  label: Incognia API
  slug: incognia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/openapi/incognia-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Incognia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Incognia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.incognia.com/api/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Incognia
provider_slug: incognia
schemes:
- description: OAuth 2.0 client-credentials grant. No scopes are defined; access is scoped by the credential's tenant.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.incognia.com/api/v2/token
  name: oauth2
  source: openapi/incognia-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: incognia-scopes
source_filename: incognia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/incognia-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/incognia-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.incognia.com/api/v2/token\n  description: OAuth 2.0 client-credentials grant. No scopes are defined; access is scoped by\n    the credential's tenant.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/scopes/incognia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cybersecurity
- Fraud Prevention
- Device Fingerprinting
- Location Identity
- Identity Verification
- Risk Assessment
- Authentication
- Fintech
- Anti-Fraud
token_urls:
- https://api.incognia.com/api/v2/token
---
