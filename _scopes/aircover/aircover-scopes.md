---
api_specs:
- filename: aircover-openapi.yml
  format: yaml
  label: Aircover Public Agent API
  slug: aircover-public-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/openapi/aircover-openapi.yml
authorization_urls:
- https://api.aircover.ai/oauth/authorize
description: ''
docs: https://www.aircover.ai/developers
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Aircover Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aircover publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aircover API on a user''s behalf.


  Tokens are issued from https://api.aircover.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aircover
provider_slug: aircover
schemes:
- description: OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration. Scopes are granted per-client and always bounded by the authenticated user's own organization permissions — an agent can never see more than the user who authorized it.
  flows:
  - authorizationUrl: https://api.aircover.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.aircover.ai/oauth/token
  name: oauth2
  source: openapi/aircover-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: 'Access the MCP tool surface only: read access to meetings, transcripts, AI agent results, deal qualification, reports, teams, and indexed documents. Does NOT grant account administration, billing, user management, or write access to CRM integrations.'
  flows:
  - authorizationCode
  scope: mcp
slug: aircover-scopes
source_filename: aircover-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.aircover.ai/.well-known/oauth-authorization-server\ndocs: https://www.aircover.ai/developers\nderived_from: openapi/aircover-openapi.yml\nissuer: https://api.aircover.ai\nschemes:\n- name: oauth2\n  source: openapi/aircover-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.aircover.ai/oauth/authorize\n    tokenUrl: https://api.aircover.ai/oauth/token\n  description: OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration.\n    Scopes are granted per-client and always bounded by the authenticated user's own organization\n    permissions — an agent can never see more than the user who authorized it.\nscopes:\n- scope: mcp\n  description: >-\n    Access the MCP tool surface only: read access to meetings, transcripts, AI agent results, deal\n    qualification, reports, teams, and indexed documents. Does NOT grant account administration, billing,\n    user\
  \ management, or write access to CRM integrations.\n  access: read\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.aircover.ai/.well-known/oauth-authorization-server (scopes_supported)\n  - openapi/aircover-openapi.yml\n  - https://www.aircover.ai/developers\npermission_model: >-\n  Layered. A token's scope caps what the client may request; every request is additionally bounded by the\n  authorizing user's own role and organization, so an agent can never see data the user could not.\n  Scopes are requested at authorization time; the developer page asks clients to request only what they\n  need. Tokens are revocable at any time via https://api.aircover.ai/oauth/revoke.\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/scopes/aircover-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Sales Enablement
- Conversation Intelligence
- Sales Coaching
- Revenue Intelligence
- AI Agents
- MCP
- Agent-Native
- CRM
- Meetings
- Transcription
- Authentication
token_urls:
- https://api.aircover.ai/oauth/token
---
