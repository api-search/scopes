---
api_specs:
- filename: parea-parea-api-openapi.yml
  format: yaml
  label: Parea AI Parea API
  slug: parea-parea-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parea/refs/heads/main/openapi/parea-parea-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Parea Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Parea AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parea AI
provider_slug: parea
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/parea-parea-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: parea-scopes
source_filename: parea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/parea-parea-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/parea-parea-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parea/refs/heads/main/scopes/parea-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- LLM
- Evaluation
- Observability
- Testing
- Prompt Management
- AI Engineering
- Machine Learning
- Tracing
- Experimentation
- Human Feedback
token_bound: false
token_urls:
- token
---
