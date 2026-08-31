---
api_specs:
- filename: hightouch-sources-api-openapi.yml
  format: yaml
  label: Hightouch Sources API
  slug: hightouch-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-sources-api-openapi.yml
- filename: hightouch-models-api-openapi.yml
  format: yaml
  label: Hightouch Models API
  slug: hightouch-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-models-api-openapi.yml
- filename: hightouch-destinations-api-openapi.yml
  format: yaml
  label: Hightouch Destinations API
  slug: hightouch-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-destinations-api-openapi.yml
- filename: hightouch-syncs-api-openapi.yml
  format: yaml
  label: Hightouch Syncs API
  slug: hightouch-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-syncs-api-openapi.yml
- filename: hightouch-campaigns-api-openapi.yml
  format: yaml
  label: Hightouch Campaigns API
  slug: hightouch-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-campaigns-api-openapi.yml
- filename: hightouch-ai-decisioning-api-openapi.yml
  format: yaml
  label: Hightouch AI Decisioning API
  slug: hightouch-ai-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-ai-decisioning-api-openapi.yml
- filename: hightouch-events-api-openapi.yml
  format: yaml
  label: Hightouch Events API
  slug: hightouch-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-events-api-openapi.yml
- filename: hightouch-identity-resolution-api-openapi.yml
  format: yaml
  label: Hightouch Identity Resolution API
  slug: hightouch-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-identity-resolution-api-openapi.yml
authorization_urls:
- https://mcp-auth.hightouch.com/oauth2/authorize
description: ''
docs: https://hightouch.com/docs/ai-integrations/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Hightouch Scopes
name_suffix: OAuth Scopes
note: 'The management REST API is API-key only and has no scope surface. OAuth exists on Hightouch''s agent surface: the A2A agent card and the workspace MCP server authenticate against https://mcp-auth.hightouch.com. The scopes below are exactly those the authorization server advertises in its RFC 8414 metadata — Hightouch publishes no per-resource scope reference page, and the agent card declares an empty scopes map, so no product-specific scopes are recorded.'
overview: 'Hightouch publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hightouch API on a user''s behalf.


  Tokens are issued from https://mcp-auth.hightouch.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hightouch
provider_slug: hightouch
schemes:
- flows:
  - authorizationUrl: https://mcp-auth.hightouch.com/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://mcp-auth.hightouch.com/oauth2/token
    tokenUrl: https://mcp-auth.hightouch.com/oauth2/token
  name: oauth2
  source: a2a/hightouch-agent-card.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in; issues an ID token (RS256).
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims about the authenticated Hightouch user.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim for the authenticated Hightouch user.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token so an agent can act beyond the initial session.
  flows:
  - authorizationCode
  scope: offline_access
slug: hightouch-scopes
source_filename: hightouch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.hightouch.com/.well-known/oauth-authorization-server\ndocs: https://hightouch.com/docs/ai-integrations/mcp\nnote: 'The management REST API is API-key only and has no scope surface. OAuth exists on Hightouch''s\n  agent surface: the A2A agent card and the workspace MCP server authenticate against https://mcp-auth.hightouch.com.\n  The scopes below are exactly those the authorization server advertises in its RFC 8414 metadata — Hightouch\n  publishes no per-resource scope reference page, and the agent card declares an empty scopes map, so\n  no product-specific scopes are recorded.'\nschemes:\n- name: oauth2\n  source: a2a/hightouch-agent-card.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp-auth.hightouch.com/oauth2/authorize\n    tokenUrl: https://mcp-auth.hightouch.com/oauth2/token\n    refreshUrl: https://mcp-auth.hightouch.com/oauth2/token\ngrant_types_supported:\n- authorization_code\n\
  - client_credentials\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\ndynamic_client_registration: https://mcp-auth.hightouch.com/oauth2/register\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issues an ID token (RS256).\n  flows:\n  - authorizationCode\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: profile\n  description: Basic profile claims about the authenticated Hightouch user.\n  flows:\n  - authorizationCode\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: email\n  description: Email claim for the authenticated Hightouch user.\n  flows:\n  - authorizationCode\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: offline_access\n  description: Issues a refresh token so an agent can act beyond the initial session.\n  flows:\n  - authorizationCode\n  sources:\n  - /.well-known/oauth-authorization-server\nauthorization_model: Beyond OAuth scopes, access is governed by Hightouch workspace RBAC — the\
  \ agent card\n  states all operations are scoped to the authenticated workspace and respect existing role-based access\n  controls. See https://hightouch.com/docs/workspace-management/roles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/scopes/hightouch-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- CDP
- Data Activation
- Reverse ETL
- Audience Management
- Identity Resolution
- Event Collection
- Marketing
- Advertising
- AI Agents
- Data Warehouse
token_urls:
- https://mcp-auth.hightouch.com/oauth2/token
---
