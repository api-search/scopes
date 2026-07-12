---
authorization_urls: []
description: ''
docs: https://docs.parea.ai/api-reference/authentication
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Parea Scopes
name_suffix: OAuth Scopes
note: Parea authenticates with a per-organization API key passed in the x-api-key header (or SDK constructor); no OAuth scopes are used or documented (https://docs.parea.ai/api-reference/authentication).
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
  source: openapi/parea-rest-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: parea-scopes
source_filename: parea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parea-rest-api-openapi.yml\ndocs: https://docs.parea.ai/api-reference/authentication\nnote: Parea authenticates with a per-organization API key passed in the x-api-key\n  header (or SDK constructor); no OAuth scopes are used or documented\n  (https://docs.parea.ai/api-reference/authentication).\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/parea-rest-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\n"
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
token_urls:
- token
---
