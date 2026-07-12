---
authorization_urls: []
description: ''
docs: https://readme.paradox.ai/reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Paradox Scopes
name_suffix: OAuth Scopes
note: Paradox does not publish OAuth scopes; the API uses an OAuth 2.0 client credentials flow (or Basic auth) with an account ID and secret key issued by the Paradox Integrations Team, with no scope parameter documented (https://readme.paradox.ai/reference/authentication).
overview: 'Paradox uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paradox
provider_slug: paradox
schemes:
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paradox-scopes
source_filename: paradox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paradox-api-openapi.yml\ndocs: https://readme.paradox.ai/reference/authentication\nnote: >-\n  Paradox does not publish OAuth scopes; the API uses an OAuth 2.0 client\n  credentials flow (or Basic auth) with an account ID and secret key issued by\n  the Paradox Integrations Team, with no scope parameter documented\n  (https://readme.paradox.ai/reference/authentication).\nschemes:\n- name: oauth2\n  source: openapi/paradox-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/scopes/paradox-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Candidate Screening
- Chatbot
- Conversational AI
- Hiring Automation
- HR Technology
- Interview Scheduling
- Recruiting
- SMS
- Talent Acquisition
token_urls:
- /auth/token
---
