---
api_specs:
- filename: openapi.json
  format: json
  label: Alloovium API
  slug: alloovium-api
  spec_type: OpenAPI
  url: https://api.alloovium.com/api/v2/openapi.json
authorization_urls:
- https://api.alloovium.com/api/v2/oauth/authorize
description: ''
docs: https://www.alloovium.com/en/developers/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alloovium Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alloovium publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alloovium API on a user''s behalf.


  Tokens are issued from https://api.alloovium.com/api/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alloovium
provider_slug: alloovium
schemes:
- flows:
  - authorizationUrl: https://api.alloovium.com/api/v2/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.alloovium.com/api/v2/oauth/token
  name: OAuth2
  version: OAuth 2.1
scope_count: 9
scope_names:
- vault:read
- vault:write
- chat:read
- chat:write
- templates:read
- templates:write
- workflows:read
- workflows:write
- meta:read
scopes:
- description: List/get projects and documents, and run vault search.
  flows:
  - authorizationCode
  scope: vault:read
- description: Create projects and upload documents.
  flows:
  - authorizationCode
  scope: vault:write
- description: List conversations and fetch conversation history.
  flows:
  - authorizationCode
  scope: chat:read
- description: Ask chat (streaming and non-streaming).
  flows:
  - authorizationCode
  scope: chat:write
- description: Poll template-fill job status.
  flows:
  - authorizationCode
  scope: templates:read
- description: Start template-fill jobs.
  flows:
  - authorizationCode
  scope: templates:write
- description: List workflows and get run status.
  flows:
  - authorizationCode
  scope: workflows:read
- description: Start workflow runs.
  flows:
  - authorizationCode
  scope: workflows:write
- description: Reserved; not currently required.
  flows:
  - authorizationCode
  scope: meta:read
slug: alloovium-scopes
source_filename: alloovium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.alloovium.com/en/developers/authentication\ndocs: https://www.alloovium.com/en/developers/authentication\nschemes:\n- name: OAuth2\n  version: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://api.alloovium.com/api/v2/oauth/authorize\n    tokenUrl: https://api.alloovium.com/api/v2/oauth/token\nscopes:\n- scope: vault:read\n  description: List/get projects and documents, and run vault search.\n  flows: [authorizationCode]\n- scope: vault:write\n  description: Create projects and upload documents.\n  flows: [authorizationCode]\n- scope: chat:read\n  description: List conversations and fetch conversation history.\n  flows: [authorizationCode]\n- scope: chat:write\n  description: Ask chat (streaming and non-streaming).\n  flows: [authorizationCode]\n- scope: templates:read\n  description: Poll template-fill job status.\n  flows: [authorizationCode]\n- scope: templates:write\n\
  \  description: Start template-fill jobs.\n  flows: [authorizationCode]\n- scope: workflows:read\n  description: List workflows and get run status.\n  flows: [authorizationCode]\n- scope: workflows:write\n  description: Start workflow runs.\n  flows: [authorizationCode]\n- scope: meta:read\n  description: Reserved; not currently required.\n  flows: [authorizationCode]\nnotes: >-\n  Dynamically registered OAuth clients are always issued read-only scopes. API keys created in the\n  Developer Console carry their own scope grant independent of OAuth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloovium/refs/heads/main/scopes/alloovium-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Company
- Construction
- Document Intelligence
- Compliance
- Artificial Intelligence
- Construction Technology
- Documents
- MCP
token_urls:
- https://api.alloovium.com/api/v2/oauth/token
---
