---
authorization_urls:
- https://vet.digitail.io/oauth/authorize
description: ''
docs: https://documentation.digitail.io/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Digitail Scopes
name_suffix: OAuth Scopes
note: Digitail's OAuth 2.0 authorization-code-with-PKCE flow does not use or document any scopes; access is granted per approved application registration (https://documentation.digitail.io/authentication).
overview: 'Digitail uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://vet.digitail.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Digitail
provider_slug: digitail
schemes:
- description: OAuth 2.0 authorization-code grant with PKCE. Bearer access token is long-lived; a refresh token is also returned.
  flows:
  - authorizationUrl: https://vet.digitail.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://vet.digitail.io/oauth/token
  name: oauth2
  source: openapi/digitail-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: digitail-scopes
source_filename: digitail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/digitail-openapi.yml\ndocs: https://documentation.digitail.io/authentication\nnote: Digitail's OAuth 2.0 authorization-code-with-PKCE flow does not use or document\n  any scopes; access is granted per approved application registration\n  (https://documentation.digitail.io/authentication).\nschemes:\n- name: oauth2\n  source: openapi/digitail-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vet.digitail.io/oauth/authorize\n    tokenUrl: https://vet.digitail.io/oauth/token\n  description: OAuth 2.0 authorization-code grant with PKCE. Bearer access token is long-lived;\n    a refresh token is also returned.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/scopes/digitail-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Veterinary
- PIMS
- Practice Management
- Pets
- Healthcare
- Scheduling
- Billing
- SaaS
token_urls:
- https://vet.digitail.io/oauth/token
---
