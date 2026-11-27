---
api_specs:
- filename: myagi-bot-contact-api-openapi.yml
  format: yaml
  label: Myagi Contact API
  slug: myagi-bot-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-contact-api-openapi.yml
- filename: myagi-bot-mcp-api-openapi.yml
  format: yaml
  label: Myagi MCP API
  slug: myagi-bot-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-mcp-api-openapi.yml
- filename: myagi-bot-well-known-api-openapi.yml
  format: yaml
  label: Myagi .well Known API
  slug: myagi-bot-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-well-known-api-openapi.yml
authorization_urls:
- https://myagi.bot/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Myagi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Myagi publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Myagi API on a user''s behalf.


  Tokens are issued from https://myagi.bot/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Myagi
provider_slug: myagi-bot
schemes:
- description: OAuth 2.0 (discovery only as of 0.1.0).
  flows:
  - authorizationUrl: https://myagi.bot/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://myagi.bot/oauth/token
  name: oauth2
  source: openapi/myagi-bot-openapi.json
scope_count: 3
scope_names:
- read:platform
- read:registry
- write:inquiry
scopes:
- description: Read platform info.
  flows:
  - authorizationCode
  scope: read:platform
- description: Read Open Agent Registry data.
  flows:
  - authorizationCode
  scope: read:registry
- description: Submit inquiries.
  flows:
  - authorizationCode
  scope: write:inquiry
slug: myagi-bot-scopes
source_filename: myagi-bot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myagi-bot-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/myagi-bot-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://myagi.bot/oauth/authorize\n    tokenUrl: https://myagi.bot/oauth/token\n  description: OAuth 2.0 (discovery only as of 0.1.0).\nscopes:\n- scope: read:platform\n  description: Read platform info.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myagi-bot-openapi.json\n- scope: read:registry\n  description: Read Open Agent Registry data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myagi-bot-openapi.json\n- scope: write:inquiry\n  description: Submit inquiries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myagi-bot-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myagi-bot/scopes/myagi-bot-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- AI Governance
- Cloud
- Governance
- Privacy
- Security
- Company
token_bound: false
token_urls:
- https://myagi.bot/oauth/token
---
