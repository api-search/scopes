---
api_specs:
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Conversational AI API
  slug: paradox-conversational-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Company API
  slug: paradox-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Candidates API
  slug: paradox-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Users API
  slug: paradox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Scheduling API
  slug: paradox-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Locations API
  slug: paradox-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Reporting API
  slug: paradox-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Candidate Attributes API
  slug: paradox-candidate-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox User Permissions API
  slug: paradox-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
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
