---
authorization_urls:
- https://{account-domain}.aha.io/oauth/authorize
description: ''
docs: https://www.aha.io/api/oauth2
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aha Scopes
name_suffix: OAuth Scopes
note: Aha! OAuth 2.0 does not define or document any scopes; access tokens inherit the full permissions of the authorizing user's account role (https://www.aha.io/api/oauth2).
overview: 'Aha.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{account-domain}.aha.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aha.io
provider_slug: aha
schemes:
- description: OAuth2 authentication with bearer tokens
  flows:
  - authorizationUrl: https://{account-domain}.aha.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{account-domain}.aha.io/oauth/token
  name: OAuth2
  source: openapi/aha-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: aha-scopes
source_filename: aha-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aha-openapi.json\ndocs: https://www.aha.io/api/oauth2\nnote: Aha! OAuth 2.0 does not define or document any scopes; access tokens inherit\n  the full permissions of the authorizing user's account role (https://www.aha.io/api/oauth2).\nschemes:\n- name: OAuth2\n  source: openapi/aha-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{account-domain}.aha.io/oauth/authorize\n    tokenUrl: https://{account-domain}.aha.io/oauth/token\n  description: OAuth2 authentication with bearer tokens\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aha/refs/heads/main/scopes/aha-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Product Management
- Roadmapping
- Idea Management
- Product Development
- Requirements
- Agile
token_urls:
- https://{account-domain}.aha.io/oauth/token
---
