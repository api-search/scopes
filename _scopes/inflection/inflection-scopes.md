---
authorization_urls: []
description: ''
docs: https://developers.inflection.ai/docs/authentication
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Inflection Scopes
name_suffix: OAuth Scopes
note: Inflection AI does not use OAuth scopes; the developer API is authenticated with bearer API keys obtained from the developer portal, and no scopes or granular permissions are documented (https://developers.inflection.ai/docs/authentication).
overview: 'Inflection AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Inflection AI
provider_slug: inflection
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: inflection-scopes
source_filename: inflection-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inflection-openapi.json\ndocs: https://developers.inflection.ai/docs/authentication\nnote: >-\n  Inflection AI does not use OAuth scopes; the developer API is authenticated with\n  bearer API keys obtained from the developer portal, and no scopes or granular\n  permissions are documented (https://developers.inflection.ai/docs/authentication).\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/scopes/inflection-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI
- LLM
- Personal AI
- Pi
- Foundation Models
- Empathetic AI
token_urls:
- token
---
