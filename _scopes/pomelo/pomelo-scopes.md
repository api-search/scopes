---
authorization_urls: []
description: ''
docs: https://developers.pomelo.la/en/api-reference/general/authorization
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Pomelo Scopes
name_suffix: OAuth Scopes
note: Pomelo's OAuth 2.0 uses the client_credentials grant (client_id, client_secret, audience only - no scope parameter), and while each API validates that the token's internally granted scopes (e.g. arg:cards:get-card in token response examples) match the required permissions, no public scopes reference is published (https://developers.pomelo.la/en/api-reference/general/authorization).
overview: 'Pomelo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.pomelo.la/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pomelo
provider_slug: pomelo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: pomelo-scopes
source_filename: pomelo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pomelo-openapi.yml\ndocs: https://developers.pomelo.la/en/api-reference/general/authorization\nnote: Pomelo's OAuth 2.0 uses the client_credentials grant (client_id, client_secret,\n  audience only - no scope parameter), and while each API validates that the token's\n  internally granted scopes (e.g. arg:cards:get-card in token response examples) match\n  the required permissions, no public scopes reference is published\n  (https://developers.pomelo.la/en/api-reference/general/authorization).\nschemes:\n- name: oauth2\n  source: openapi/pomelo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/scopes/pomelo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fintech
- Card Issuing
- Embedded Finance
- Payments
- Latin America
token_urls:
- https://auth.pomelo.la/oauth/token
---
