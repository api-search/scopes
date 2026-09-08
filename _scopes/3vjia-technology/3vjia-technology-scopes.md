---
api_specs:
- filename: 3vjia-technology-open-platform-openapi.yml
  format: yaml
  label: 3vjia Open Platform API
  slug: 3vjia-technology-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/openapi/3vjia-technology-open-platform-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: 3Vjia Technology Scopes
name_suffix: OAuth Scopes
note: 'The OAuth 2.0 client_credentials grant on graph.3vjia.com defines NO scopes — the token carries the whole contracted surface and authorisation is enforced by what the enterprise''s contract enables, not by scope. No type: OAuthScopes pointer is emitted in apis.yml, because there is no scope surface to point at; authentication/3vjia-technology-authentication.yml carries the auth model. This file records the verified zero.'
overview: '3vjia Technology uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://graph.3vjia.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 3vjia Technology
provider_slug: 3vjia-technology
schemes:
- description: OAuth 2.0 client credentials. appId/appKey are issued after developer + application approval at https://dev.3vjia.com/manage/my-app/developer. Token TTL 7200s; re-requesting invalidates the previous token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://graph.3vjia.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/3vjia-technology-open-platform-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: 3vjia-technology-scopes
source_filename: 3vjia-technology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/3vjia-technology-open-platform-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/3vjia-technology-open-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://graph.3vjia.com/oauth/token\n  description: OAuth 2.0 client credentials. appId/appKey are issued after developer + application\n    approval at https://dev.3vjia.com/manage/my-app/developer. Token TTL 7200s; re-requesting\n    invalidates the previous token.\nscopes: []\nscope_count: 0\napis_yml_pointer: none\nnote: >-\n  The OAuth 2.0 client_credentials grant on graph.3vjia.com defines NO scopes — the token carries the\n  whole contracted surface and authorisation is enforced by what the enterprise's contract enables, not\n  by scope. No type: OAuthScopes pointer is emitted in apis.yml, because there is no scope surface to\n  point at; authentication/3vjia-technology-authentication.yml carries the auth model.\
  \ This file records\n  the verified zero.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/scopes/3vjia-technology-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- 3D Design
- Home Furnishing
- Interior Design
- Manufacturing
- Custom Furniture
- CAD
- Rendering
- Artificial Intelligence
- SaaS
- China
- Open Platform
token_urls:
- https://graph.3vjia.com/oauth/token
---
